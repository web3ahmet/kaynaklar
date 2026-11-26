# Test sonucun yalan söylüyor olabilir: sızıntı kontrol listesi

Çıkmış soruları ezberleyen öğrenci denemede tam puan alır, gerçek sınavda takılır. Modeller de aynısını yapar: overfitting. Verinin bir dilimini teste saklamak bunu çoğu zaman yakalar. Ama test verisine eğitimden bilgi sızarsa (data leakage) test de yalan söyler.
Kaynak: https://scikit-learn.org/stable/common_pitfalls.html

## Kontrol listesi
- [ ] **Aynı kişi iki yerde mi?** Aynı müşteri, hasta ya da kullanıcı hem eğitimde hem testte varsa, model onu tanır. Bölmeyi kişiye göre yap.
- [ ] **Tarih karıştı mı?** Tarihli veriyi rastgele bölersen model geleceği görmüş olur. Eskiyle eğit, yeniyle test et.
- [ ] **Hazırlık nerede yapıldı?** Ölçekleme, eksik değer doldurma gibi işlemleri bütün veriye değil, yalnız eğitim kısmına göre ayarla.
- [ ] **Cevabı ele veren sütun var mı?** Sonradan oluşan bir bilgi (ör. "iade edildi mi") tahmin edilecek şeyi ele veriyor olabilir. Çıkar.
- [ ] **Sonuç fazla mı iyi?** Beklenmedik derecede yüksek skor genelde sızıntı işaretidir. Sevinmeden önce kontrol et.
- [ ] **Model neye bakıyor?** Modelin kararını hangi özelliklere dayandırdığına bak. Anlamsız bir ipucuna yaslanıyor olabilir. Kaynak: https://arxiv.org/abs/1602.04938

Video: https://youtube.com/shorts/RvQlcQCB6GA
