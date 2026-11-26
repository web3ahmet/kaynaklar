# Uzun bir yığını Claude'a ayıklatmak: şablon + kontrol adımları

Biri bir podcast'in onlarca bölümünü Claude'a verip işe yarayan tavsiyeleri tek bir rehbere çevirmiş (kişinin kendi paylaşımı, bağımsız doğrulamadım). Anthropic'in kendi çalışmasında yığın çok daha büyük: yaklaşık 950 ajan, 21 saatte 200 bin kadar enzim dizisini 3.500 adaya, sonra 20 rapora indirmiş (https://www.anthropic.com/news/claude-discovers-novel-enzyme-system). İkisinde ortak olan şu: büyük bir yığın Claude'da daralıyor, son kontrolü insan yapıyor.

## Hangi yığınlar uygun?
- Dinlediğin bir podcast'in ya da izlediğin bir serinin yazıya dökülmüş hâli.
- Aylardır biriken not dosyaların.
- Bir konuda topladığın makaleler ya da e-postalar.
- Toplantı kayıtlarının yazıya dökülmüş hâli.

## Adım adım
1. **Topla:** Hepsini tek klasöre koy, dosya adlarına tarih ya da bölüm numarası ver.
2. **Parçala:** Çok büyükse 5-10 dosyalık gruplara böl. Her grubu ayrı ver, sonunda özetleri birleştir.
3. **Ayıklat:** Aşağıdaki şablonu kullan.
4. **Kontrol et:** En az 3 maddeyi kaynağına geri dönüp kendin doğrula.

## Ayıklama şablonu (Claude'a)
"Sana [kaç] tane [podcast bölümü / not / makale] veriyorum. Amacım: [tek cümle, ör. ilk işini arayan biri için yol haritası].
1. Her dosyadan bu amaca hizmet eden somut tavsiyeleri çıkar.
2. Her tavsiyenin yanına hangi dosyadan geldiğini yaz.
3. Birden fazla dosyada geçenleri birleştir, kaç kez geçtiğini belirt.
4. Sonunda tek sayfalık bir rehber yaz: en çok tekrar edenler üstte.
5. Emin olmadığın ya da kaynakta açıkça yazmayan bir şeyi ekleme."

## Kontrol listesi
- [ ] Her maddenin yanında kaynak dosya yazıyor mu?
- [ ] Rastgele 3 maddeyi açıp kaynağında gerçekten öyle mi geçiyor diye baktın mı?
- [ ] Rehberde kaynakta olmayan, "kulağa doğru gelen" bir genelleme var mı?
- [ ] Çelişen tavsiyeler varsa Claude ikisini de göstermiş mi, yoksa birini seçip öbürünü silmiş mi?

Enzim örneğinde de son söz insanda: yeni sistemin ne işe yaradığı henüz bilinmiyor, laboratuvar deneylerini insanlar yaptı.

Videonun tamamı: https://youtu.be/04_N1KMI5JA
