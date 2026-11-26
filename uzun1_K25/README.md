# Context window ve token: yeni başlayan için tek sayfa

Yapay zekayla uzun uzun yazışınca bir noktadan sonra cevaplar neden kötüleşiyor? Cevap iki kelimede: context window ve token. Resmi açıklama burada: https://platform.claude.com/docs/en/build-with-claude/context-windows

## İki kelime, kısaca
- **Context window (bağlam penceresi):** Yapay zekanın o sohbette aynı anda "aklında tutabildiği" her şey. Senin mesajların, onun cevapları, eklediğin dosyalar hepsi bu pencereye girer.
- **Token:** Pencerenin ölçü birimi. Yazdığın metin parçalara bölünür, her parça bir token. Metin uzadıkça token sayısı artar.
- **Ücret:** Kullandıkça ödenen planlarda fatura token üzerinden hesaplanır. Fiyatlar: https://platform.claude.com/docs/en/about-claude/pricing
- **Pencere boyutu** modele ve sürüme göre değişir. Videoda söylediğim değer bugünkü Claude modelleri için; güncel rakamı her zaman resmi sayfadan kontrol et.

## Pencere dolunca ne oluyor?
Claude Code pencere dolmadan eski konuşmayı kendisi özetliyor, yani hafıza taşmıyor. Ama özet, ayrıntının bir kısmını kaybeder. Bir de sohbette konular birbirine karıştıysa, yapay zeka her cevapta o karışık geçmişin hepsini yeniden okuyor. Kalite buradan düşüyor.

## Bağlamı belli bir seviyede tutmak için
- [ ] Yeni bir konuya geçiyorsan yeni bir sohbet aç.
- [ ] Bir iş bittiyse, sonraki işe başlamadan önce kısa bir özet yazdır ve yeni sohbete o özetle başla.
- [ ] Büyük dosyanın tamamını değil, gereken kısmını ver.
- [ ] Aynı açıklamayı her seferinde baştan yazıyorsan, onu bir kez dosyaya koy ve oradan okut.
- [ ] Claude Code'da `/clear` sohbeti sıfırlar, `/compact` eskiyi özetleyip yer açar.

## 3 adımlık deneme (kendi işinde)
1. Her gün yaptığın tek bir işi seç (ör. bir e-postayı özetletmek, bir listeyi düzenletmek).
2. Aynı işi iki şekilde yap: bir kez uzamış, karışık bir sohbetin içinde; bir kez temiz, yeni bir sohbette.
3. İki cevabı yan yana koy: hangisi daha doğru, hangisi daha az düzeltme istedi? Bir hafta not tut, sana en verimli geleni kural yap.

Bu benim yöntemim, resmi bir kural değil. Senin işinde en iyi sonucu veren ölçü, kendi testinden çıkar.

Videonun tamamı: https://youtu.be/XcI1w3J3hcU
