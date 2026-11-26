# SSD neden yıpranır, ömrüne nasıl bakarsın?

## Kısaca nasıl çalışıyor?
- Her hücre yalıtılmış küçük bir bölmede elektron tutar; yük yıllarca kalır.
- Yazma küçük gruplarla (sayfa) olur, silme ise koca bir blokta, toptan.
- Bu yüzden SSD bir düzeltmeyi eskisinin üstüne yazmaz: yeni bir yere yazar, eskisini sonra temizler.
- Her silme hücreyi biraz yıpratır.

## Hücre türleri ve yaklaşık ömür (yazma/silme döngüsü)
| Tür | Hücre başına bit | Yaklaşık döngü |
|---|---|---|
| SLC | 1 | ~50-100 bin |
| MLC | 2 | ~3-10 bin |
| TLC | 3 | ~1-3 bin |
| QLC | 4 | ~150-1000 |

Bunlar üretici/sektör tahmini, standart bir değer yok (kaynak: https://www.ssstc.com/knowledge-detail/nand-flash-types-comparison/ , https://lexarenterprise.com/comparing-nand-flash-slc-mlc-tlc-qlc-industrial-application/). Diskinin gerçek değeri için üreticinin verdiği **TBW** (toplam yazılabilir terabayt) değerine bak.

## Kendi diskini kontrol et
- [ ] Disk modelini bul, üreticinin sayfasında TBW ve garanti süresine bak.
- [ ] Üreticinin kendi aracını kullan ya da smartmontools ile `smartctl -a <disk>` çalıştır (https://www.smartmontools.org). "Percentage Used" ya da "Wear Leveling" satırı ne kadar yıprandığını gösterir.
- [ ] Diski ağzına kadar doldurma; boş alan, SSD'nin temizlik işini rahatlatır.
- [ ] Önemli dosyaların yedeği başka bir yerde de olsun. SSD ne kadar sağlam olursa olsun, yedek şart.

## Yapay zekâya sor
"smartctl çıktımı aşağıya yapıştırıyorum. Diskimin ne kadar yıprandığını ve dikkat etmem gereken bir satır olup olmadığını teknik bilmeyen birine anlat."

Video: https://youtube.com/shorts/0lX4zzHYpQo
