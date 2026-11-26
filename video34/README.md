# Tohum (seed): aynı "rastgele" sonucu tekrar almak

Bilgisayar rastgele sayıyı bulmaz, formülle üretir. Bütün dizi tek bir başlangıç sayısına bağlıdır: tohum (seed). Aynı tohumu verirsen aynı diziyi alırsın.
Kaynak: https://docs.python.org/3/library/random.html

## Örnek kod (Python)
```python
import random

random.seed(42)
print(random.sample(range(100), 5))
```
Bu kodu kaç kez çalıştırırsan çalıştır, aynı 5 sayıyı verir. `random.seed(42)` satırını silersen her seferinde farklı sayılar gelir.

## Ne zaman tohum ver?
- [ ] Rapor ya da test için örneklem alıyorsan: aynı sonucu tekrar üretebilmek için.
- [ ] Bir arkadaşın aynı sonucu görmeli diyorsan: tohumu kodla birlikte paylaş.

## Ne zaman verme?
- [ ] Şifre, güvenlik kodu gibi tahmin edilmemesi gereken şeyler için `random` modülünü hiç kullanma. Python belgesi bunun için `secrets` modülünü önerir.

## Yapay zekâya sor
"Bu kodda rastgelelik nerede kullanılıyor? Sonuçları tekrar üretilebilir yapmak için tohumu nereye koymam gerekir? [kodu yapıştır]"

Video: https://youtube.com/shorts/s804bdm_Iqk
