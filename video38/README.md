# Yavaş sorgu: önce neye bakarsın?

İşlemci toplama işinde çok hızlı. Sorgu yavaşsa suçlu çoğu zaman toplama değil, veriyi işlemcinin önüne getirmek. Bu yüzden önce ne kadar veri okuduğuna bak.
Büyük sorguları binlerce işlemciye bölen ve tabloyu sütun sütun saklayan sistemin makalesi: https://research.google/pubs/dremel-interactive-analysis-of-web-scale-datasets-2/

## Sırayla bak
- [ ] **1. Kaç sütun okuyorsun?** `SELECT *` yerine yalnız gereken sütunları yaz. Sütun sütun saklanan tablolarda okunan veri buna göre azalır.
- [ ] **2. Kaç satır okuyorsun?** Tarih ya da başka bir filtreyle yalnız gereken satırları al. Filtreyi mümkün olduğunca erken uygula.
- [ ] **3. Birleştirmeler (JOIN):** Birleştirme sonrası satır sayısı beklediğinden çok mu arttı? Eşleşen anahtarı kontrol et.
- [ ] **4. Aynı işi tekrar mı yapıyorsun?** Her seferinde ham veriden hesaplamak yerine ara sonucu bir tabloya kaydet.
- [ ] **5. Sorgu planına bak:** Kullandığın veritabanı sorgu planı ya da yürütme ayrıntısı gösteriyorsa, en çok zamanı hangi adımın aldığına bak.

## Yapay zekâya sor
"Bu sorgu yavaş çalışıyor. Hangi kısmı en çok veri okuyor olabilir? Sonucu değiştirmeden okunan veriyi azaltacak değişiklikleri öner ve her birini açıkla: [sorguyu yapıştır]"

Video: https://youtube.com/shorts/pScxKse9-g4
