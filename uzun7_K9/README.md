# Ajanlar arası devir notu + hatadan kontrole

Videoda işleri bölüşen ayrı Claude'lar (ajanlar) var. Her biri işini bitirince arkasından gelene bir not bırakıyor; yeni başlayan, bir öncekinin kaldığı yerden devam ediyor.

## Devir notu kalıbı
Ajan işini bitirirken şu 4 satırı kendi not dosyasının **sonuna ekler** (üzerine yazmaz):
```
## tarih · iş
- Yapıldı: …
- Açık kalan: …
- Dikkat: … (bir sonraki ajanın bilmesi gereken tuzak)
```

## Hatadan kontrole 4 adım
- [ ] **1. Fark et:** Hatayı Claude'a somut söyle (ör. "ekrandaki yazılar birbirine çok yakın").
- [ ] **2. Deftere yazdır:** "Hatanın nedenini hata defterine tek satır yaz."
- [ ] **3. Tekrar ederse ölç:** "Bunu her seferinde ölçen küçük bir kontrol yaz" (ör. yazılar arasındaki boşluğu ölçen kontrol).
- [ ] **4. Kontrolü kapıya koy:** İş, kontrol geçmeden bitmiş sayılmasın.

Videonun tamamı: {YT_LINK}
