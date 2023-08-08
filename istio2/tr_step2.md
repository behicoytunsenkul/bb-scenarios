### Istio Kullanımı
Istio, kubernetes üzerinde çalışan uygullamaların trafiğini yönetmek amacıyla Kubernetes'in default network konfigürasyonunu **by-pass** eder. Uygulamaların pod'larına kendisine ait sidecar proxy container'larına ekler ve tanımlayacağı network, security gibi kurallarını bu proxy'ler üzerinden çalıştırır.

> **Sidecar Proxy Container:** Mikroservis mimarileri ve service mesh çözümlerinde sıklıkla kullanılan bir kavramdır. Asıl amacı main container ile aynı host ortamında çalışan ve hizmetin ağ trafiğini yönetmek, kontrol etmek ve daha güvenli bir hale getirmek gibi önemli görevleri üstlendir.

Istio'u kullanmaya başlamadan önce bir takım konfigürasyon ayarlamalarının yapılması gerekmektedir. İlk olarak size tahsis edilen makinenize aşağıdaki komutu girin:
````
istioctl proxy-status
````
Proxy yapılandırması için aşağıdaki yönergeleri takip edebilirsiniz.

**1)** Belirli bir pod'daki Envoy örneği için küme yapılandırması ile ilgili bilgi almak için aşağıdaki komutu kullanabilirsiniz:
````
istioctl proxy-config cluster <pod-name> [flags]
````
**2)** Belirli bir pod'daki Envoy örneği için önyükleme yapılandırması hakkında bilgi almak için aşağıdaki komutu kullanabilirsiniz:
````
istioctl proxy-config bootstrap <pod-name> [flags]
````
**3)** Belirli bir pod'daki Envoy örneği için listener yapılandırması hakkında bilgi almak için aşağıdaki komutu kullanabilirsiniz:
````
istioctl proxy-config listener <pod-name> [flags]
````
**4)** Belirli bir pod'daki Envoy örneğinin route yapılandırması hakkında bilgi almak için aşağıdaki komutu kullanabilirsiniz:
````
istioctl proxy-config route <pod-name> [flags]
````
**5)** Belirli bir pod'daki Envoy örneği için end-point yapılandırması hakkında bilgi almak için aşağıdaki komutu kullanabilirsiniz:
````
istioctl proxy-config endpoints <pod-name> [flags]
````

