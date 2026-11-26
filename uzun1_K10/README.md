# Agent'ı ne zaman kapatmalı? Kontrol listesi + devir notu şablonu

Model büyük bir context window'a sahip olabilir (https://platform.claude.com/docs/en/build-with-claude/context-windows), ama hepsini tek işe doldurmak şart değil. Ben agent'ı ortalama 200 bin token civarında kapatıp temiz bağlamla yenisini açıyorum; bu benim yöntemim, resmi bir kural değil. Sebep: biriken her şey aynı işle ilgili değil ve her token'ın fiyatı var.

## Kapatma zamanı geldi mi?
- [ ] Konu değişti (yeni bir işe geçiyorsun).
- [ ] Agent eski bir kararı ya da dosyayı karıştırmaya başladı.
- [ ] Aynı hatayı ikinci kez yaptı.
- [ ] Cevaplar yavaşladı, fatura büyüdü.
- [ ] Bir aşama bitti, sonraki aşamanın eski ayrıntıya ihtiyacı yok.

İkisi ya da daha fazlası işaretliyse: devir notu yazdır, kapat, yenisini aç.

## Devir notu şablonu (agent'a yazdır)
"Bu oturumu kapatmadan önce şu başlıklarla kısa bir devir notu yaz:
1. Amaç: ne yapmaya çalışıyoruz?
2. Yapılanlar: bitenler, dosya adlarıyla.
3. Kararlar: neyi neden seçtik?
4. Açık işler: sırada ne var?
5. Dikkat: yanlış yapılmaması gereken şeyler."

Yeni agent'a ilk mesaj olarak bu notu ver.

Videonun tamamı: https://youtu.be/XcI1w3J3hcU
