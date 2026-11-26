# Agent ile skill farkı + ilk skill şablonu

## Fark tek cümlede
Agent kim olduğunu bilir, skill işin nasıl yapılacağını.

- **Agent:** Bir rol. Claude Code'da `.claude/agents/` altında bir Markdown dosyası. İçinde "sen kimsin, ne yaparsın" yazar.
- **Skill:** Bir işin detaylı talimatı. `.claude/skills/skill-adi/SKILL.md` dosyası. Aynı prompt'u her seferinde baştan yazmazsın.
- Agent tanımındaki `skills` alanı, o skill'i agent'a yükler.

Kaynak: https://code.claude.com/docs/en/sub-agents · https://code.claude.com/docs/en/skills

## İlk skill şablonu
Dosya yolu: `.claude/skills/haftalik-ozet/SKILL.md`

```
---
name: haftalik-ozet
description: Haftalık notları 5 maddelik özete çevirir. Kullanıcı "haftalık özet" istediğinde kullan.
---

# Haftalık özet

## Adımlar
1. Verilen notları oku.
2. En önemli 5 olayı seç.
3. Her birini tek cümleyle yaz.

## Kurallar
- Notta olmayan bir şeyi ekleme.
- Emin olmadığın yeri "belirsiz" diye işaretle.
```

## Kontrol
- [ ] `description` ne zaman kullanılacağını açıkça söylüyor mu? Claude skill'i buna bakarak seçer.
- [ ] Adımlar başka biri okuyunca da anlaşılır mı?

Videonun tamamı: https://youtu.be/XcI1w3J3hcU
