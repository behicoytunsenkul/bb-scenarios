### 4- Assembly Dili için Ortam Kurulumları
Eğitimimiz süresince terminal üzerinde Assembly dili ile kodlama yapabilmemiz için **NASM** kurulumu yapmamız gerekmektedir. Ancak birçok programlama diline nazaran Assembly, Linux'a kurulu bir şekilde gelmektedir. 
 Sisteminizde NASM kurulu olup olmadığını öğrenmek için aşağıdaki komutu terminale giriniz:
 ```
 whereis nasm
 ```
 Yukarıdaki komutu çalıştırdıktan sonra terminal ekranında ``nasm: /usr/bin/nasm`` çıktı alıyorsanız sisteminizde nasm kurulu anlamına gelmektedir. Ancak sadece ``nasm:`` şeklinde bir çıktı alıyorsanız, sisteminizde nasm kurulu olmadığı anlamına gelir. Sisteminize nasm kurabilmek için aşağıdaki komutları sırayla giriniz:
 ```
 apt-get update
 apt-get install nasm
 ```
 Yukarıdaki komutları çalıştırdıktan sonra ``whereis nasm`` komutu ile nasm kurulumu gerçekleşip gerçekleşmediğini kontrol edebilirsiniz.
 
> Kurulumları başarılı bir şekiilde gerçekleştirdikten sonraki adıma geçerek, **Hello World** uygulamamızı kodlamaya başlayalım.ss