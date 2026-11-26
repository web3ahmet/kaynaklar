# Cookie ve session'ı güvenle saklamak: 5 madde

Giriş yaptığında sunucu sana rastgele bir numara (session kimliği) verir; cookie'de taşınan da o numaradır. Bu numarayı ele geçiren, şifreni bilmeden senin yerine giriş yapmış gibi olur. O yüzden onu şifre gibi koru.
Kaynak: https://developer.mozilla.org/en-US/docs/Web/HTTP/Guides/Cookies

## 5 madde
- [ ] **1. Koda yazma:** Cookie'yi script'in içine yapıştırma. Ayrı bir dosyada ya da ortam değişkeninde tut.
- [ ] **2. Git'e girmesin:** O dosyayı `.gitignore`'a ekle. Bir kez commit edilen cookie'yi değiştirmeden güvende sayma.
- [ ] **3. Loga basma:** Hata mesajlarında ve loglarda cookie ya da session değeri görünmesin.
- [ ] **4. Süresi dolunca yenile:** Cookie'nin bir son kullanma tarihi olabilir. Süresi dolunca script sessizce bozulmasın; hata versin, sen yeniden giriş yap.
- [ ] **5. Ayrı hesap:** Mümkünse otomasyon için yalnız gereken yetkisi olan ayrı bir hesap kullan.

## Sızdığını düşünürsen
- [ ] Siteden çıkış yap ve şifreni değiştir; çoğu site bununla eski oturumları kapatır.

Video: https://youtube.com/shorts/vgKQt4JSamo
