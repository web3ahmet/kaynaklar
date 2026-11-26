# Çin'in ucuz modelleri: denemeden önce 4 kontrol

Videodaki fiyat ve sıralamalar 18 Kasım 2026 verisi; bu alanda her hafta bir şey değişiyor. O yüzden rakamı videodan değil, aşağıdaki sayfalardan kendin kontrol et.
Güncel kullanım sıralaması: https://openrouter.ai/rankings

## Fiyat ve bilgi sayfaları
- GLM-5.3 Flash (Z.ai): https://docs.z.ai/guides/overview/pricing
- MiniMax M3.1 Flash: https://platform.minimax.io/docs/guides/pricing
- Hy4 Flash (Tencent), çıkış haberi: https://technode.com/2026/11/16/tencent-launches-hy4-flash-cutting-ai-task-costs-by-95-in-internal-tests/
- MiMo-V2.6 Pro (Xiaomi), çıkış haberi: https://siliconangle.com/2026/09/22/xiaomi-introduces-mimo-v2-6-series-open-source-ai-model-family/

Not: Videodaki GLM fiyatını ikincil bir kaynaktan aldık; resmi sayfadan teyit et.

## "15 sente 50 sent" ne demek?
Model fiyatı milyon token başına iki rakamla yazılır. İlki senin gönderdiğin metin (giriş), ikincisi modelin yazdığı cevap (çıkış). "15 sente 50 sent" demek: 1 milyon token gönderirsen 0,15 dolar, 1 milyon token cevap alırsan 0,50 dolar.

## "320 milyar parametre, 18 milyarı çalışıyor" ne demek?
Model birçok küçük uzmana bölünmüş gibi düşün. Her soruda hepsi değil, yalnız o soruya uygun birkaçı çalışıyor. Daha az hesap yapıldığı için hızlı ve ucuz.

## Denemeden önce 4 kontrol
- [ ] **1. Fiyat:** Giriş ve çıkış fiyatını resmi sayfadan oku. İndirimli dönem varsa bitiş tarihine bak.
- [ ] **2. Lisans:** "Open weight" ya da "MIT" yazıyorsa modeli kendi bilgisayarına ya da sunucuna indirip çalıştırabilirsin. "Söz verildi" yazıyorsa henüz yok demektir.
- [ ] **3. Verin nereye gidiyor:** API'ye gönderdiğin metin o şirketin sunucusuna gider. Şifre, müşteri bilgisi, kişisel veri yapıştırma.
- [ ] **4. Küçük bir testle başla:** Aynı soruyu hem bu modele hem de tanıdığın bir modele sor, cevapları yan yana koy. Ucuz model senin işinde yeterliyse ondan sonra büyüt.

Videonun tamamı: https://youtu.be/0vzzUASeVZY
