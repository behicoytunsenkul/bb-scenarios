### 1) Istio Kurulumu
Bir önceki eğitimimizde **Istio**'nun ne olduğunu ve neden kullanıldığını incelemiştik. Şimdi ise Kubernetes üzerine Istio kurulumunun nasıl gerçekleştirildiğine bakacağız. Hazırsanız başlayalım 🚀

İlk olarak size tahsil edilen makine üzerinden Istioctl'in son release'ni kurmak için aşağıdaki komutu girin:
````
curl -L https://istio.io/downloadIstio | sh -
````
Ek olarak, belirli bir versiyonunu kurmak isterseniz aşağıdaki komutu kullanabilirsiniz:
````
curl -L https://istio.io/downloadIstio | ISTIO_VERSION=1.3.0 sh -
````

Istioctl'i kurduğumuza göre Trafik Yönetimi örneğinde kullanacağımız demo profili ile Istio kurmak için aşağıdaki komutu girin:
````
istioctl manifest apply --set profile=demo
````
Yukarıdaki komut demo profilinde yer alan bütün component'leri Kubernetes cluster'ına kuracaktır. Kurulan component'leri aşağıdaki komut ile inceleyebilirsiniz:
````
kubectl get all -n istio-system
````

--> Istio kurulumunu başarılı bir şekilde tamamladığımıza göre bir sonraki adıma yani Istio ile trafik yönetimine geçebiliriz.