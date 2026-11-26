# OpenRouter sıralaması ve DeepSeek fiyatı nasıl okunur

OpenRouter, tek bir hesapla birçok yapay zeka modeline bağlanmanı sağlayan bir aracı. Hangi modele ne kadar istek gittiğini de herkese açık bir sıralamada gösteriyor. Videodaki rakamlar (DeepSeek V4.1 Flash, 30 günde 222 trilyon token, haftalık isteklerin yüzde 31,8'i) 18 Kasım 2026 verisi; sıralama her hafta değişiyor.
Kaynak: https://openrouter.ai/rankings

## 3 adımda oku
- [ ] **1. Sıralamaya bak:** https://openrouter.ai/rankings sayfasında süreyi seç (haftalık ya da aylık). Üstteki model en çok token işleyen model. Bu "en zeki" demek değil, "en çok kullanılan" demek.
- [ ] **2. Fiyatı resmi sayfadan kontrol et:** https://api-docs.deepseek.com/quick_start/pricing. Fiyat milyon token başına iki rakamla yazılır: ilki senin gönderdiğin metin (giriş), ikincisi modelin cevabı (çıkış). "15 sente 60 sent" demek: 1 milyon token gönderirsen 0,15 dolar, 1 milyon token cevap alırsan 0,60 dolar. Yoğun saatlerde fiyat farklı olabilir, sayfada ayrıca yazıyor.
- [ ] **3. Lisansa bak:** "Open weight" ve "MIT" yazıyorsa modeli kendi bilgisayarına ya da sunucuna indirip çalıştırabilirsin. Popülerliğinin bir sebebi de bu.

## Dikkat
API'ye gönderdiğin metin o şirketin sunucusuna gider. Şifre, müşteri bilgisi, kişisel veri yapıştırma. Önce zararsız küçük bir işle dene.

Resmi site: https://www.deepseek.com

Videonun tamamı: https://youtu.be/0vzzUASeVZY
