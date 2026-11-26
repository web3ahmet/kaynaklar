# "Yetkisiz" hatası: token kontrol listesi

Çoğu otomasyonda iki token var:
- **Access token:** Her istekte kapıda gösterdiğin kart. Kısa ömürlüdür.
- **Refresh token:** Yalnız yeni access token istemek için kullanılır. Otomasyonu ayakta tutan budur.

Kaynak: https://www.rfc-editor.org/rfc/rfc6749 · https://www.rfc-editor.org/rfc/rfc6750

## Sırayla bak
- [ ] **1. Access token'ın süresi doldu mu?** Doldu ve otomasyon yenisini istemiyorsa hata buradan gelir.
- [ ] **2. Refresh token hâlâ geçerli mi?** Bazı servislerde belli bir süre kullanılmayınca ya da şifre değişince geçersiz olur.
- [ ] **3. Yeni refresh token kaydedildi mi?** Bazı servisler her yenilemede yeni bir refresh token verir ve eskisini geçersiz kılar. Yenisini kaydetmiyorsan bir sonraki sefer hata alırsın. Kaynak: https://www.rfc-editor.org/rfc/rfc9700
- [ ] **4. Erişim geri alındı mı?** Hesap ayarlarından uygulamanın izni kaldırılmış olabilir.
- [ ] **5. Yetki kapsamı (scope) değişti mi?** Otomasyonun yeni bir iş için ek izne ihtiyacı olabilir.

## Güvenlik
- [ ] Token'ları koda yazma, loga basma, git'e koyma. Şifre gibi sakla.

## Önlem
- [ ] Yenileme başarısız olunca sana haber gelsin; bozulmayı başkası fark etmeden önce sen gör.

Video: https://youtube.com/shorts/_aQwLAW0sa8
