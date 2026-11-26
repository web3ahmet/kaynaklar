# Ajana iş tarif ederken açık kapı bırakma

Bir yapay zekâ tekne yarışını bitirmek yerine bir koyda daire çizdi; çünkü puan yoldaki hedeflerden geliyordu. Makine ödülü kastettiğin gibi değil, yazdığın gibi okur.
Kaynak: https://openai.com/index/faulty-reward-functions/

## Kontrol listesi
- [ ] **Asıl hedef yazılı mı?** "Puanı artır" değil, "yarışı bitir" gibi gerçekten istediğin sonucu yaz.
- [ ] **Kestirme yol var mı?** Ajan hedefi işi yapmadan nasıl tutturabilir? Bir dakika düşün, aklına gelen yolu kapat.
- [ ] **Yapmaması gerekenler:** Dokunmaması gereken dosyalar, silmemesi gereken şeyler, harcamaması gereken para.
- [ ] **Bitti ne demek?** İşin bittiğini neyle anlayacaksın? Ölçülebilir yaz.
- [ ] **Takılınca ne yapsın?** "Emin değilsen dur ve bana sor" cümlesini ekle.
- [ ] **Sonucu sen kontrol et:** Ajanın "bitti" demesi yetmez; çıktıya kendin bak.

## Örnek görev tanımı
"Görev: Bu klasördeki 20 faturanın tutarlarını bir tabloya aktar.
Bitti demek: 20 satır, her satırda tarih, firma ve tutar var; toplam, faturaların toplamıyla aynı.
Yapma: Fatura dosyalarını değiştirme, silme ya da taşıma. Okuyamadığın tutarı tahmin etme.
Takılırsan: O faturayı 'okunamadı' diye işaretle ve devam et; sonunda listesini bana ver."

Video: https://youtube.com/shorts/XriDJAumlsM
