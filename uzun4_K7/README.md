# Context kontrol listesi + prompt şablonu

Model 2 şeyle cevap verir: eğitimden gelen genel bilgiyle ve o an önüne konan context'le. Context, modelin o an gördüğü her şey: arka plandaki talimatlar (system prompt), proje dosyan, önceki mesajlar, araç çıktıları.
Resmi belge: https://docs.anthropic.com/en/docs/build-with-claude/context-windows

## Sormadan önce
- [ ] **Amaç:** Bu cevapla ne yapacaksın? Bir cümleyle yaz.
- [ ] **Malzeme:** Model hangi dosyaya, metne ya da tabloya bakmalı? Ekle.
- [ ] **Kurallar:** Uyması gereken şeyler: uzunluk, dil, ton, dokunmaması gereken yerler.
- [ ] **Örnek:** Beğendiğin bir cevap örneği var mı? Ekle.
- [ ] **Gereksiz olanı çıkar:** İlgisiz uzun metin dikkati dağıtır. Sadece işe yarayanı ver.

## Prompt şablonu
"Amaç: [bu cevapla ne yapacağım].
Elindeki malzeme: [dosya/metin].
Kurallar: [uzunluk, ton, dokunma dediğin yerler].
Örnek: [beğendiğin bir cevap].
Bilmediğin bir şey olursa uydurma, bana sor."

Videonun tamamı: https://youtu.be/3dHoxEFW0lA
