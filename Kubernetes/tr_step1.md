## 3- Kubernetes Nasıl Kurulur?
 Sistemimize Kubernetes, kurabilmemiz için ilk olarak Docker uygulamasının tüm Centos sunucularına yüklenmesi gerekmektedir. Ancak bizim sistemimizde Docker kurulu bir şekilde geldiği için herhangi bir kurulum işlemi gerçekleştirmiyoruz.
 >Kişisel cihazınızda Dokcer kurulumları için Docker eğitim serimizden yardım alabilirsiniz.
 
 Kubernetes eğitimimizin ilk dersinde **kubeadm**, **kubelet** ve **kubectl** araçlarının kurulumlarını gerçekleştireceğiz. Bunun ilk önce sistemimize ``curl`` kurabilmek için aşağıdaki komutu terminale giriniz:
 ```
 yum install curl -y
 ```
 ``curl`` kurulumu başarılı bir şekilde tamamlandıktan sonra Kubernetes repository'ini tüm sunuculara eklememiz gerekiyor. Bunun için ilk olarak bir dosya oluşturmamız gerekiyor:
 ```
 vi /etc/yum.repos.d/kubernetes.repo
 ```
 Dosyayı oluşturduktan sonra, dosyayı kapatarak terminal ekranına geri dönebilirsiniz. Şimdi ise az önce bahsetmiş olduğumuz **Kubernetes Araçları**nı kurmaya başlayabiliriz.
 
 --> Kubernetes eğitimimizin bir sonraki adımına geçiş yapabilirsiniz.
 s