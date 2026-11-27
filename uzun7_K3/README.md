# SessionStart hook'u: hazır istem + kurmadan önce 4 soru

Hook, Claude Code'da belli bir anda senin belirlediğin bir işi otomatik yapan özellik. SessionStart oturum açılırken çalışıyor ve ürettiği metin Claude'un önüne konuyor. Video hazırlanırken bu metnin sınırı 10.000 karakterdi; güncel değeri belgeden kontrol et.
Kaynak: https://code.claude.com/docs/en/hooks

## Hazır istem
"Bu projede oturum açılırken çalışan bir SessionStart hook'u kur. Hook şu dosyanın ilk kısmını Claude'un önüne koysun: <dosya adı>. Metin kısa kalsın. Kurmadan önce bana hook'un ne yaptığını, hangi dosyayı okuduğunu ve hangi komutu çalıştırdığını sade bir dille anlat; ben onaylamadan kurma."

## Kurmadan önce sor
- [ ] **1. Ne çalıştırıyor?** Hook'un çalıştırdığı komutu satır satır açıklat.
- [ ] **2. Neyi okuyor?** Hangi dosyaya eriştiğini ve dışarıya bir şey gönderip göndermediğini sor.
- [ ] **3. Ne kadar uzun?** Önüne koyduğu metin sınırın çok altında mı? Her şeyi koyma, önemli olan kaybolur.
- [ ] **4. Nasıl kapatırım?** Sorun çıkarsa hook'u nasıl devre dışı bırakacağını öğren.

## Güvenlik
Hook senin bilgisayarında, senin yetkinle çalışıyor. İnternetten kopyaladığın bir hook'u ne yaptığını bilmeden kurma.

Videonun tamamı: {YT_LINK}
