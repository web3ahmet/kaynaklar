# İlk otomasyonun: başlangıç şablonu

Sohbette işi sen yaparsın, otomasyonda sistem yapar. İlk adım araç seçmek değil, işi parçalamak.

## 1. Tek bir iş seç
Her gün ya da her hafta elle yaptığın, 10 dakikadan kısa, hep aynı adımlarla ilerleyen bir iş. Örnekler:
- Gelen e-postalardan faturaları bir klasöre ayırmak
- Takvimdeki yarının toplantılarını sabah kendine mesaj atmak
- Bir formdan gelen cevapları tabloya eklemek

## 2. Üçe böl
| Parça | Soru | Örnek |
|---|---|---|
| **Trigger (tetik)** | Ne olunca başlıyor? | Yeni e-posta geldi |
| **Step (adım)** | Arada ne yapılıyor? | Ekte fatura var mı bak, varsa tarihini oku |
| **Output (çıktı)** | Sonunda ne oluşuyor? | Dosya klasörde, tabloya bir satır |

## 3. Karar gereken yeri işaretle
Adımlardan birinde "bunu okuyup anlamak lazım" diyorsan, yapay zekâ orada devreye girer. Gerisi düz kural.

## 4. Kontrol listesi
- [ ] Yanlış giderse kimse zarar görmüyor mu? (İlk otomasyonda para ve başkasına mesaj yok.)
- [ ] Önce birkaç gün çıktıyı yalnız sana göstersin, sonra kendi yapsın.
- [ ] Hata olunca sana haber veriyor mu?

## Prompt örneği
"Her gün elle yaptığım şu işi otomasyona çevirmek istiyorum: [işi yaz]. Bunu trigger, adımlar ve output olarak böl; hangi adımda yapay zekâ kararı gerektiğini işaretle; n8n'de hangi node'larla kurulabileceğini sırala."

Videonun tamamı: https://youtu.be/XcI1w3J3hcU
