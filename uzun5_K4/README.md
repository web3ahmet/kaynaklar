# Ajandan kanıt iste: prompt kalıbı + "bulamadım" kontrolü

Bağımsız bir testte REA büyük bir uygulamada 421 JavaScript dosyasını yaklaşık 52 saniyede taradı. Ama 2 preload dosyasını kaçırdı ("0" dedi); başka bir aramada da "eşleşme yok" dedi. Bulamamak, yokluğun kanıtı değil.
Kaynak: https://hackernoon.com/i-tested-rea-githubs-viral-reverse-engineering-tool-on-a-real-electron-app

## Prompt kalıbı
"Cevabını verirken her iddia için kanıtını yaz: hangi dosya, hangi fonksiyon, hangi satır. Kanıt gösteremediğin bir şeyi 'emin değilim' diye işaretle. Bir şey bulamazsan hangi dosyalara baktığını ve hangilerine bakmadığını listele."

## "Bulamadım" dediğinde
- [ ] **1. Nereye baktı?** Taradığı klasörlerin ve dosya türlerinin listesini iste.
- [ ] **2. Neyi atladı?** "Hangi dosyalara bakmadın?" diye sor. Gizli, küçük ya da farklı uzantılı dosyalar sık atlanır.
- [ ] **3. Farklı kelimeyle ara:** Aynı şeyi başka bir isimle ya da kısaltmayla tekrar arat.
- [ ] **4. Bir örnekle dene:** Var olduğunu bildiğin bir şeyi arat. Onu da bulamıyorsa arama yöntemi eksik.
- [ ] **5. İpucu gibi oku:** Sonucu kesin bilgi gibi değil, kontrol edeceğin bir ipucu gibi değerlendir.

Videonun tamamı: https://youtu.be/IAL8F-lCOyY
