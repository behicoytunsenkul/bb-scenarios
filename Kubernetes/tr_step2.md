## 4- Kubernetes Araçları ve Kurulumları
Kubernetes araçlarının kurulumlarına geçmenden önce ilk olarak bu araçların ne için kullanıldığını inceleyelim:
**a) kubeadm:** Kubernetes Cluster kurmanıza yardımcı olan bir araçtır.
**b) kubelet:** Node'u API sunucusuna kaydetneye yardımcı olan ve her Node üzerinde çalışabilen bir araçtır.
**c) kubectl:** Kubernetes Cluster'ı kontrol edebileceğiniz bir komut satırı aracıdır.
Şimdi ise aşağıdaki komutu terminale girerek bu araçların kurulumlarını gerçekleştirelim:
```
yum install kubeadm kubectl kubelet -y
```
Kurulumlar başarılı bir şekilde tamamlandıktan sonra, ilk kubelet aracını başlatarak aktif bir hale getirelim:
```
systemctl start kubelet
systemctl enable kubelet
```
Sonrasında ``swapoff -a`` komutunu terminale girerek swap'i devre dışı bırakmamız gerekiyor.

-> Yukarıdaki işlemleri başarılı bir şekilde tamamladıktan sonra diğer kubernetes araçları ile işlemler yapacağımız, eğitimimizin son adımına geçiş yapabilirsiniz.