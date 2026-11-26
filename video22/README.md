# Docker mı, Kubernetes mi? 5 soru + otomatik yeniden başlatma

## Çöken container'ı Docker'a kaldırt
Docker'da container'ı başlatırken bir yeniden başlatma kuralı (restart policy) verebilirsin. Container çökerse Docker onu kendisi yeniden başlatır, ama yalnız o tek makinenin içinde.

```
docker run -d --restart unless-stopped benim-ajanim
```

- `no`: varsayılan, yeniden başlatmaz.
- `on-failure`: yalnız hatayla kapanırsa başlatır.
- `always`: her durumda başlatır.
- `unless-stopped`: sen elle durdurmadıysan başlatır.

Kaynak: https://docs.docker.com/engine/containers/start-containers-automatically/

## Kubernetes ne ekliyor?
"Bu uygulamadan 3 tane hep ayakta olsun" dersin; Kubernetes bunu birden çok makinede sürekli kontrol eder, eksik olanı yeniden kurar.
Kaynak: https://kubernetes.io/docs/concepts/overview/ · https://kubernetes.io/docs/concepts/architecture/controller/

## Başlamadan 5 soru
- [ ] **1.** Uygulamam tek makinede mi çalışıyor? Evetse büyük olasılıkla Docker yeter.
- [ ] **2.** Makinenin kendisi kapanırsa iş durmalı mı, devam etmeli mi?
- [ ] **3.** Aynı anda birden çok kopya çalışması gerekiyor mu?
- [ ] **4.** Bu sistemi kim bakımda tutacak? Kubernetes öğrenme ve bakım yükü getirir.
- [ ] **5.** Çökünce bana haber gelecek mi? Yeniden başlatma sorunu gizler, çözmez; loglara bak.

Video: https://youtube.com/shorts/XXOiDUbEmw4
