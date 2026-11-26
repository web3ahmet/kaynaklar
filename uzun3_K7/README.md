# Model seçerken iki sayı: zekâ puanı ve gerçek maliyet

Videodaki örnek (Kasım 2026, Artificial Analysis): GPT-6.2 Astra API'de Fable'la aynı liste fiyatında (milyon token başına 8 dolar girdi, 40 dolar çıktı), zekâ puanında Fable'ın 3 puan gerisinde; ama sitenin maliyet hesabında Fable yaklaşık 26 dolar, Astra 4 dolar. Günlük iş modeli GPT-6.2 Sol 57 puan, yaklaşık 1 dolar. Sayılar hızlı değişir; güncelini https://artificialanalysis.ai üzerinden kendin kontrol et.

## Neden liste fiyatı yetmiyor?
Aynı fiyattaki iki model aynı işi farklı sayıda token harcayarak bitirebilir. Fatura token sayısı × fiyat olduğu için asıl soru "bu iş bana kaça patladı?"

## 4 adımda karşılaştır
1. Aday 2-3 modeli seç (biri güçlü, biri günlük iş modeli).
2. Artificial Analysis'te her biri için **zekâ puanını** ve sitenin **maliyet hesabını** yan yana yaz.
3. Kendi işinden 5 gerçek örnekle küçük bir test yap; sonuçların yeterli olup olmadığına bak.
4. Yeterli olan en ucuz modeli seç; zor işler için güçlüyü yedekte tut.

## Kontrol listesi
- [ ] Liste fiyatına değil, iş başına maliyete baktım.
- [ ] Puan farkı benim işimde fark ediliyor mu, test ettim.
- [ ] Sayıların tarihini not ettim (bu rehberdekiler Kasım 2026).

## Prompt örneği
"Şu 5 örnek görevi [görevler] iki modelle çalıştırdım, çıktılar aşağıda. Hangisi yeterli? Yeterli olan en ucuz seçeneği gerekçesiyle söyle."

Videonun tamamı: https://youtu.be/0vzzUASeVZY
