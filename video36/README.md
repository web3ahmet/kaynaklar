# Bilgisayar 1 biti nasıl hatırlar? (tek sayfa)

## Fikir
Bir bilgiyi tutmak için onu kendine durmadan tekrar edersin. Devre de aynısını yapar: bir kapının çıkışı ötekinin girişine, onunki de ilkine bağlanır. Bu döngü, bir kez kurulan değeri kendi kendine tekrar ederek tutar.

## 3 adımda latch (mandal)
1. İki NOR kapısı al, çıkışlarını çapraz bağla (A'nın çıkışı B'ye, B'ninki A'ya).
2. **S (set)** girişine kısa bir 1 ver → çıkış 1 olur ve sen S'yi bıraksan da 1 kalır.
3. **R (reset)** girişine kısa bir 1 ver → çıkış 0'a döner ve öyle kalır.

Latch "şeffaftır": izin verildiği sürece girişteki her değişikliği hemen içeri alır.

## Flip-flop farkı
Flip-flop değeri yalnız **clock** sinyalinin tek bir anında (genelde yükselen kenarda) alır. Arada giriş ne kadar oynarsa oynasın çıkış sabit kalır. İşlemcinin binlerce parçası aynı tempoda adım atabilsin diye register'lar bu yüzden flip-flop'tan yapılır.

## Kontrol listesi
- [ ] Döngü var mı? Yoksa hafıza da yok.
- [ ] Değer ne zaman içeri giriyor: izin süresince mi (latch), tek bir anda mı (flip-flop)?
- [ ] S ve R aynı anda 1 olursa ne olur? (SR latch'te yasak durum; tasarımda kaçınılır.)

## Kendin dene
Bir yapay zekâ sohbetine şunu yaz:
"İki NOR kapısıyla SR latch'i doğruluk tablosuyla anlat. Sonra D flip-flop'un yükselen kenarda nasıl farklı davrandığını 3 örnek zaman adımıyla göster."

Video: https://youtube.com/shorts/k_ayMmOLuns
