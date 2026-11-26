# Ajana para ya da yetki vermeden önce 5 sınır

Anthropic'in Project Deal deneyinde 69 çalışana birer Claude ajanı ve 100 dolar bütçe verildi; ajanlar kendi aralarında pazarlık edip 186 anlaşma yaptı. Zayıf modelle temsil edilenler kaybettiklerini fark etmedi (kaynak: https://www.anthropic.com/features/project-deal). Ders basit: ajan adına konuşuyorsa, sınırı sen çizersin.

## 5 sınır
1. **Bütçe tavanı:** tek işlemde ve toplamda en fazla ne kadar harcayabilir? Rakamla yaz.
2. **Onay eşiği:** hangi tutarın üstünde ya da hangi tür işte önce sana sorsun?
3. **Kapsam:** neyi alıp satabilir, kimlerle konuşabilir? Listede yoksa yapamaz.
4. **Kayıt:** her teklifi, karşı teklifi ve gerekçeyi yazsın; sonradan okuyabil.
5. **Durdurma düğmesi:** tek komutla bütün işlemleri durdurabiliyor musun?

## Kontrol listesi
- [ ] İlk denemede gerçek para yerine küçük bir test bütçesi.
- [ ] Ajanın sonucunu bir kez de kendin kontrol et; "iyi anlaşma" dediği gerçekten iyi mi?
- [ ] Karşı tarafta da bir ajan olabilir; daha güçlü modelin ondan daha iyi pazarlık edebileceğini hesaba kat.

## Prompt örneği
"Benim adıma şu işi pazarlık et: [iş]. Toplam bütçe [X], tek teklif en fazla [Y]. [Z] tutarını geçen her teklifte dur ve bana sor. Her adımı gerekçesiyle kaydet."

Videonun tamamı: https://youtu.be/04_N1KMI5JA
