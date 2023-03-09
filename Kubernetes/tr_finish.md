## 6- kubectl Aracının Kullanımı
Komut satırı aracı olan kubectl bir çok özelliği de beraberinde getirmektedir. Bu özellikleri tek tek inceleyelim:
**A->** namespace'te çalışan tüm pod'ları listeler:
```
kubectl get po --all-namespaces
```
**B->** cluster'daki tüm pod'ları listeler:
```
kubectl get ns
```
**C->** cluster'daki tüm node'ları listeler:
```
kubectl get nodes
```

Gibi birçok özelliği bize sunmaktadır.

--> Tebrikler. Kubernetes eğitimini başarılı bir şekide tamamladınız. Senaryoyu sonlandırarak bir sonraki Kubernetes eğitimimize geçiş yapabilirsiniz.s