# IPv4 ve IPv6: tek sayfa

## Fark
| | IPv4 | IPv6 |
|---|---|---|
| Uzunluk | 32 bit | 128 bit |
| Görünüş | `192.168.1.10` | `2001:db8::1` |
| Adres sayısı | yaklaşık 4,3 milyar | IPv4'ün 2⁹⁶ katı |

- 3 Şubat 2011'de IPv4 adreslerinin ana havuzu (IANA) boşaldı. Kaynak: https://www.arin.net/blog/2011/02/03/iana-ipv4-free-pool-depletion
- IPv6 adres yapısı: https://www.rfc-editor.org/rfc/rfc4291
- Cihazın, takip edilmeyi zorlaştırmak için zaman zaman geçici IPv6 adresleri kullanabilir: https://www.rfc-editor.org/rfc/rfc8981
- UUID de tam 128 bit: https://www.rfc-editor.org/rfc/rfc9562

## Kendi IPv6 bağlantını kontrol et
Harici bir siteye girmene gerek yok; bilgisayarın kendisi söyler.
- [ ] **Windows:** Komut İstemi'ni aç, `ipconfig` yaz. "IPv6 Address" satırına bak.
- [ ] **Mac:** Terminal'i aç, `ifconfig` yaz. `inet6` ile başlayan satırlara bak.
- [ ] **Nasıl okunur?** Yalnız `fe80` ile başlayan adres varsa bu sadece yerel ağ adresidir. `2` ya da `3` ile başlayan bir adres görüyorsan, internet sağlayıcın sana büyük olasılıkla genel bir IPv6 adresi vermiştir.
- [ ] Emin olamazsan internet sağlayıcına "hattımda IPv6 açık mı?" diye sor.

Video: https://youtube.com/shorts/JNVXDnhnZ68
