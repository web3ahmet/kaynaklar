# Packet switching: bir mektup örneğiyle

## Kısa tarih
- ARPANET'te ilk mesaj 29 Ekim 1969'da UCLA'dan SRI'ye gönderildi. "login" yazılacaktı; yalnız "lo" gitti, sonra sistem çöktü. Yaklaşık 1 saat sonra tamamı gitti. (https://en.wikipedia.org/wiki/ARPANET)
- "Nükleer savaşa dayanmak için kuruldu" hikâyesi ARPANET için doğru değil; asıl amaç bilgisayarları paylaşmaktı. Söylenti, RAND'ın dayanıklı haberleşme çalışmasından geliyor. (https://www.internetsociety.org/internet/history-internet/brief-history-internet/)

## Fikir: uzun mektubu kartpostallara böl
1. 10 sayfalık bir mektubu 10 kartpostala yaz.
2. Her kartpostala "1/10, 2/10..." diye numara ve alıcı adresi koy.
3. Kartpostallar farklı postanelerden, farklı yollardan gidebilir.
4. Alıcı numaralara bakıp sırayı kurar; eksik olanı yeniden ister.

İnternette bu kartpostallara **packet** denir. Bir yol tıkanırsa paketler başka yoldan gider; tek bir hat tüm konuşmayı kilitlemez.

## Bugün nerede görürsün?
- [ ] Video izlerken kısa bir takılma: bazı paketler geç geldi.
- [ ] Büyük bir dosyayı indirirken yüzde yüzde ilerleme: paketler sırayla birikiyor.
- [ ] Mesaj uygulamasında "gönderiliyor..." yazısı: paketler henüz ulaşmadı.

## Yapay zekâya sor
"Bir WhatsApp mesajı telefonumdan arkadaşımın telefonuna giderken kaç parçaya bölünebilir ve yolda neler olur? Teknik bilmeyen birine anlat."

Video: https://youtube.com/shorts/zGMCT0IJjHA
