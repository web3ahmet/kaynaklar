# REA'yı kurmadan önce: kontrol listesi

REA (Reverse Engineer Anything), derlenmiş bir programı ajana okutmayı kolaylaştırıyor. Yeni bir decompiler değil: Hopper, Ghidra, IDA gibi eski araçları ajana sürdüren bir köprü. Resmi depo yaklaşık 469 bin yıldızda (19 Kas 2026, GitHub API; https://github.com/morluto/rea). Lisans MIT.

## 1. Doğru yerden mi indiriyorsun?
- [ ] Resmi README'ye göre meşru olanlar yalnız: `github.com/morluto/rea`, `rea.tools` ve npm paketi `rea-agents`.
- [ ] "rea-tools" adlı sahte bir depo trojan olarak işaretlendi (VirusTotal'da 45 motordan 8'i). Benzer isimlere tıklama.
- [ ] Kurulum resmi README'deki komutla: `npx rea-agents setup` (Node 22+).

## 2. Neyi kurcalıyorsun?
- [ ] Yalnız kendi dosyan ya da incelemene izin verilen bir program.
- [ ] Önce depodaki `DISCLAIMER.md` dosyasını oku.
- [ ] Hukuk: AB 2009/24 Yazılım Direktifi (md. 5/3 ve 6) ve 5846 sayılı FSEK md. 38 gözlemleme, inceleme ve test etmeye belli koşullarda izin veriyor; kopyalamaya izin vermiyor. Bu hukuki tavsiye değil.

## 3. Güvenli kurulum
- [ ] Mümkünse sanal makinede (VM) çalıştır.
- [ ] Ajanı salt okuma modunda tut; dosyayı değiştirmesine izin verme.
- [ ] Çıkan kodu kopyalayıp başka yerde kullanma.

## 4. Rapora nasıl bakmalı?
- [ ] Ajan "bulamadım" diyorsa bu, o şeyin olmadığı anlamına gelmez. Bulamamak yokluğun kanıtı değil.

## İlk soru örneği
"Bu programın açılışta hangi dosyaları okuduğunu ve internete bağlanıp bağlanmadığını özetle. Hiçbir dosyayı değiştirme, emin olmadığın yere 'doğrulanmadı' yaz."

Videonun tamamı: https://youtu.be/IAL8F-lCOyY
