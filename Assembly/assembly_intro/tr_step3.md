```
mov eax,4
mov ebx,1
mov ecx,msg
mov edx,13
int 0x80
```
Bu kısım, Linux sistem çağrısını kullanarak msg değişkeninde depolanan "Hello World" metnini ekrana yazdırmak için gerekli adımları içerir. Şimdi bu adımları inceleyelim:
* **mov eax,4** -> Yazdırma işlemi için sistem çağrısı numarasını eax kaydediyor. 4, yazdırma işlemi için write sistem çağrısı numarasıdır.
* **mov ebx,1** -> Ekrana yazdırmak için kullanılacak dosya tanıtıcısıdır. 1, standart çıkış dosyasının dosya tanıtıcısıdır.
* **mov ecx,msg** -> Yazdırılacak mesajın bellek adresini ecx kaydeder.
* **mov edx,13** -> Yazdırılacak bayt sayısını belirtir. 13 bayt, "Hello World" dizisindeki karakterlerin sayısıdır.
* **int 0x80** ->  Sistem çağrısını tetikler ve eax kaydedilen sistem çağrısı numarasına bağlı olarak işlem yapar. Bu durumda, write sistem çağrısı, eax kaydedilmiş olduğu için tetiklenir ve mesaj yazdırılır.

```
mov eax,1
xor ebx,ebx
int 0x80
```
Kodumuzun son kısmı ise, programın sonlandırılmasını sağlayan adımları içermektedir. Şimdi bu adımları sırayla inceleyelim:
* **mov eax,1** -> Programın sonlandırılması için kullanılacak sistem çağrısı numarasını eax kaydediyor. 1, exit sistem çağrısı numarasıdır.
* **xor ebx,ebx** -> Çıkış kodunu 0 olarak ayarlamak için kullanılır. Bu, programın başarıyla sonlandığını gösterir.
* **int 0x80** -> Sistem çağrısını tetikler ve eax kaydedilen sistem çağrısı numarasına bağlı olarak işlemi gerçekleştirir.

> Assembly dilinde yapmış olduğumuz ilk uygulamayı nasıl çalıştıracağımızı öğreneceğimiz son adıma geçiş yapabilirsiniz.