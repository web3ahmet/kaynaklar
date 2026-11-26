# TV reklamlarını AI'la kapatmadan önce: 5 adımlık güvenli kontrol listesi

İnsanlar akıllı TV'lerindeki reklamları ve gereksiz uygulamaları Claude Code gibi ajanlarla kapatıyor. Haber: https://techcrunch.com/2026/10/19/people-are-using-ai-to-make-their-smart-tvs-dumb-again/
Bu işlerde ajan genelde ADB (Android Debug Bridge) denen bağlantıyı kullanır. Resmi belge: https://developer.android.com/tools/adb

## 5 adım
- [ ] **1. Yedek:** Başlamadan önce TV'de yüklü uygulamaların listesini bir dosyaya kaydettir. Neyi kapattığını sonra bu listeden görürsün.
- [ ] **2. Önce sor, sonra yap:** Ajana "komutları çalıştırmadan önce bana tek tek göster" de. Her komutu sen onayla.
- [ ] **3. Sil değil, devre dışı bırak:** Uygulamayı kaldırmak yerine kapatmayı (disable) iste. Geri dönmesi çok daha kolay.
- [ ] **4. Geri alma komutu:** Her adım için "bunu nasıl geri alırım" komutunu da yazdır ve sakla.
- [ ] **5. İşin bitince bağlantıyı kapat:** TV'de açtığın geliştirici ayarını ve ağ üzerinden hata ayıklamayı kapat.

## Dikkat
- Garanti, güncelleme ve üretici koşulları markadan markaya değişir; kendi TV'nin koşullarına bak.
- Ajan senin verdiğin yetkiyle çalışır. Onay vermeden komut çalıştırmasına izin verme.

## Başlamadan sor
"TV'mde reklam gösteren uygulamaları bulmak istiyorum. Hiçbir şeyi değiştirmeden önce yüklü uygulamaları listele, hangisinin ne işe yaradığını açıkla ve her değişiklik için geri alma komutunu da yaz."

Videonun tamamı: https://youtu.be/04_N1KMI5JA
