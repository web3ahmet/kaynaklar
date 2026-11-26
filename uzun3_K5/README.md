# Claude'da hangi iş, hangi model?

Videodaki sayılar Kasım 2026: Arena'nın genel sıralamasında ilk 10'da 7 kez Claude vardı (https://arena.ai). Ailenin en tepesi Fable 5.2, milyon token başına girdi 8, çıktı 40 dolar. Fiyatlar değişir; güncelini https://claude.com/pricing sayfasından kontrol et.

## Kural: en güçlüsünü değil, yetenini seç
| İş | Model seçimi |
|---|---|
| Kısa soru, çeviri, e-posta taslağı, özet | Ailenin küçük ve hızlı modeli |
| Günlük çalışma: belge yazmak, kod düzeltmek, araştırmayı toparlamak | Orta model (çoğu işin varsayılanı) |
| Çok adımlı, zor, hatası pahalı iş: uzun plan, karmaşık kod, ince analiz | En güçlü model (Fable) |

## 4 soruluk karar
1. Bu işi orta model dün bir kez yapabildi mi? Evetse büyüğe geçme.
2. Hata yaparsa bedeli ne? Yüksekse güçlü model + kendi kontrolün.
3. Aynı işi günde kaç kez yapacaksın? Sık tekrarlanıyorsa ucuz model kazandırır.
4. Cevap uzun mu olacak? Çıktı token'ı girdiden pahalı; uzun çıktılarda fark büyür.

## Kontrol listesi
- [ ] Varsayılan modelim orta model.
- [ ] Güçlü modeli yalnız zor işte açıyorum.
- [ ] Ayda bir fiyat sayfasına bakıp tabloyu güncelliyorum.

## Prompt örneği
"Şu işi yapacağım: [iş]. Bunu küçük, orta ya da en güçlü modelle yapmak arasında seçim yap; gerekçeni hata bedeli ve tekrar sıklığına göre açıkla."

Videonun tamamı: https://youtu.be/0vzzUASeVZY
