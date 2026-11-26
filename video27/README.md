# E-posta geç düşüyorsa: telefon ayarları kontrol listesi

## Neden oluyor?
- **iPhone:** Düşük Güç Modu açıkken posta kontrolü ve arka planda uygulama yenileme (Background App Refresh) kapanır (https://support.apple.com/en-us/101604).
- **Android:** ekran kapalı, telefon hareketsiz ve şarjda değilken **Doze** devreye girer; ağ erişimi askıya alınır, zamanlanmış işler bir sonraki "bakım penceresine" ertelenir (https://developer.android.com/training/monitoring-device-state/doze-standby).

## iPhone'da bak
- [ ] Ayarlar > Pil: Düşük Güç Modu açık mı? Önemli bir e-posta bekliyorsan kapat.
- [ ] Ayarlar > Genel > Arka Planda Uygulama Yenileme: posta uygulaman açık mı?
- [ ] Posta hesabının ayarında yeni veriyi alma yöntemi: "Push" mu, saatlik "Fetch" mi?

## Android'de bak
- [ ] Pil tasarrufu açık mı?
- [ ] Uygulamalar > e-posta uygulaman > Pil: "Kısıtlanmamış" ya da "Optimize edilmemiş" seçeneği var mı?
- [ ] Uygulamanın bildirim izni açık mı?

(Menü adları telefona ve sürüme göre değişebilir.)

## Otomasyon dersi
İki yol var: **sormak** (her saat kutuya bak, yani polling) ya da **haber beklemek** (zil çalınca bak, yani push/webhook). Kendi otomasyonlarında da aynı seçimi yaparsın: sık sormak pil ve kota yer, haber beklemek daha hızlı ama karşı tarafın haber vermesine bağlı.

## Yapay zekâya sor
"Telefonum [model, sürüm]. E-postalar geç geliyor. Kontrol etmem gereken ayarları menü yollarıyla sırala."

Video: https://youtube.com/shorts/xmJ9wK1p5gA
