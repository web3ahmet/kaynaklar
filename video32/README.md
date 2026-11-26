# Aynı sorgu neden ikinci kez anında gelir? BigQuery önbelleği (tek sayfa)

## Fikir
Sık lazım olan bir şeyi her seferinde arşivden çıkarmazsın, masana not olarak yapıştırırsın. Bilgisayar da aynısını yapar: sık istenen veriyi en yakın yerde tutar. Bu yakın kopyanın adı önbellek (cache).

BigQuery bunu sorgu sonuçlarına uyguluyor. Bir sorguyu çalıştırınca sonucu geçici bir tabloya yazıyor. Aynı kişi, aynı projede, birebir aynı sorguyu tekrar çalıştırırsa baştan hesaplamıyor, hazır sonucu veriyor.

## Bilmen gereken 3 şey
1. **Süre:** Kopya genelde 24 saat kadar duruyor. Garantisi yok, daha erken de silinebilir.
2. **Ücret:** Önbellekten gelen sorgu için ücret alınmıyor ve çok daha hızlı geliyor. Kotadan yine de sayılıyor.
3. **Kimin:** Kopya senin kullanıcına ve projene ait. (Enterprise sürümlerde aynı projedeki başka birinin sonucundan da yararlanabiliyorsun.)

## Önbellek ne zaman kullanılmaz?
- Sorgu metni herhangi bir şekilde değiştiyse: tek bir boşluk ya da yorum bile.
- Sorgudaki tablolardan biri (ya da view) değiştiyse.
- Tabloya az önce canlı (streaming) veri eklendiyse.
- Sorgu o anın saatini, tarihini ya da rastgele bir sayı istiyorsa (`CURRENT_TIMESTAMP`, `CURRENT_DATE`, `RAND` gibi).
- Sonucu kendi belirlediğin bir tabloya yazdırıyorsan.
- Sorgu birden çok tabloyu joker karakterle (`tablo_*`) okuyorsa.
- Kopyanın süresi dolduysa.

## Hız ölçerken önbelleği kapat
Önbellek açıkken ölçtüğün hız gerçek değil, ikinci çalıştırma neredeyse hep "anında" görünür.
- **Konsol:** sorgu editöründe *Edit* > *Query settings* > *Cache preference* altında **Use cached results** işaretini kaldır. (Arayüz güncellenirse menü adı değişebilir; ayar adı aynı kalır.)
- **bq komut satırı:** `--nouse_cache` ekle.
- **API:** `configuration.query.useQueryCache = false`.

## Sonuç önbellekten mi geldi? Nasıl anlarsın
- **Konsol:** sorgu sonucunda *Job information* sekmesine bak. "Bytes processed" satırı **0 B (results cached)** diyorsa önbellekten geldi.
- **API:** iş bilgisinde `cacheHit` alanı `true` ise önbellekten geldi.

## Kontrol listesi
- [ ] Hız ya da maliyet ölçüyorum: önbellek kapalı mı?
- [ ] Pano bazen yavaş, bazen anında açılıyor: arada tablo yenilenmiş olabilir mi?
- [ ] Sorgu saat/tarih fonksiyonu içeriyor mu? İçeriyorsa her seferinde baştan hesaplanır.

## Kendin dene
Aynı sorguyu iki kez çalıştır, iki seferin süresine ve "Bytes processed" satırına bak. Sonra sorguya tek bir boşluk ekle ve tekrar çalıştır, ne değişti?

Resmî belge: https://docs.cloud.google.com/bigquery/docs/cached-results

Video: https://youtube.com/shorts/2sRUop8B2MU
