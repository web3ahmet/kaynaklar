# İlk agent'ına rol yaz: hazır kalıp

Agent ayrı bir program değil; yapay zekânın kendisi, sadece ona bir rol ve sınır veriyorsun. Ofisteki gibi: biri mühendis, biri muhasebeci. Claude Code'da her sub-agent kendi bağlamıyla çalışır (https://code.claude.com/docs/en/sub-agents).

## Kalıp (4 satır)
1. **Kimsin:** "Sen ... işini yapan bir asistansın."
2. **Ne yaparsın:** yapacağı iş, adım adım.
3. **Ne yapmazsın:** sınırlar (dosya silme, para harcama, dışarıya mesaj atma gibi).
4. **Çıktın ne:** hangi biçimde teslim edeceği (madde listesi, tablo, kısa özet).

## Örnek 1: e-posta ayıklayıcı
"Sen gelen e-postaları ayıklayan bir asistansın. Her e-postayı 'acil / bu hafta / bilgi' diye etiketle. Cevap yazma, hiçbir şeyi silme. Çıktın: 3 başlık altında konu satırları."

## Örnek 2: toplantı özetçisi
"Sen toplantı notlarını özetleyen bir asistansın. Kararları ve kimin neyi ne zamana yapacağını çıkar. Notta olmayan bir şey ekleme; emin olmadığın yere 'belirsiz' yaz. Çıktın: 5 maddeyi geçmeyen liste."

## Kontrol listesi
- [ ] Rol tek bir işe odaklı mı? (5 ayrı sekme gibi: her biri kendi işi.)
- [ ] "Ne yapmazsın" satırı yazıldı mı?
- [ ] Çıktı biçimi belli mi?
- [ ] Önce 3 gerçek örnekle denedin mi?

Videonun tamamı: https://youtu.be/XcI1w3J3hcU
