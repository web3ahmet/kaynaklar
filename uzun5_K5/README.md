# MCP başlangıç notu: aracı ajana bağlamadan önce

## MCP nedir?
MCP (Model Context Protocol), bir AI ajanının dışarıdaki araçlarla konuşmasını sağlayan ortak bir bağlantı yolu. Ajan soruyu alır, MCP üzerinden aracı çalıştırır, sonucu geri alıp sana anlatır.
Resmi site: https://modelcontextprotocol.io

## Videodaki örnek
REA, Ghidra gibi tersine mühendislik araçlarını MCP üzerinden Claude Code, Codex ve Cursor gibi ajanlara bağlıyor. Yeni bir decompiler değil; ajanla eski araçlar arasında bir köprü. Kaynak kodu geri getirmiyor; elde ettiğin şey sözde kod ve onun yorumu.
- REA: https://github.com/morluto/rea
- Ghidra: https://en.wikipedia.org/wiki/Ghidra

## Bağlamadan önce sor
- [ ] **Kim yazmış?** Bu MCP sunucusu resmi kaynaktan mı geliyor?
- [ ] **Neye erişiyor?** Dosyalarına, internete, hesaplarına mı? Gerekenden fazlası varsa bağlama.
- [ ] **Okuma mı, yazma mı?** Sadece okuyor mu, yoksa bir şeyi değiştirebiliyor, silebiliyor mu?
- [ ] **Onay istiyor mu?** Ajan aracı çalıştırmadan önce sana soruyor mu? Sormuyorsa bu ayarı aç.
- [ ] **Nerede çalışıyor?** Kendi bilgisayarında mı, başka bir sunucuda mı? Verin nereye gidiyor?

Videonun tamamı: https://youtu.be/IAL8F-lCOyY
