# Kendi Claude hafızanı kurarken 6 tavsiye

Kaynaklar: https://code.claude.com/docs/en/memory · https://code.claude.com/docs/en/hooks · https://obsidian.md/help/data-storage

## Kontrol listesi
- [ ] **1. Düzeltmeyi kurala çevir:** Claude'u her düzelttiğinde "bunu kurallara ekle" de.
- [ ] **2. Oturum başında okut:** Bunu bir SessionStart hook'u kurdurarak yapabilirsin; kurmadan önce ne yaptığını sade bir dille anlatmasını iste.
- [ ] **3. Oturum sonu kartı:** Her oturumun sonunda 3 satır yazdır: ne yaptın, ne kaldı, sıradaki adım ne.
- [ ] **4. Tekrar eden hataya kontrol:** Aynı hata 2 kez olduysa bir kural daha ekleme; onu ölçen küçük bir kontrol iste.
- [ ] **5. Gizli bilgi yok:** Şifreni, anahtarını bu klasöre koyma; kişisel notlarını ayrı tut.
- [ ] **6. Hazır rehberi körü körüne uygulatma:** Hook senin yetkinle çalışıyor; ne çalıştırdığını bilmeden kurma.

## Obsidian?
Şart değil. Claude klasörü doğrudan okuyor; Obsidian'ı notlar arasında gezmek için sonradan ekleyebilirsin.

Videonun tamamı: {YT_LINK}
