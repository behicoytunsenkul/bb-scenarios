### 6- Uygulamamızı Çalıştıralım
**hello.asm** dosyamız içerisine yazdığımız komutların hepsini incelediğimize göre, uygulamamızı çalıştırma adımına geçiş yapabiliriz.
İlk olarak aşağıdaki komutu, terminal ekranımıza girelim:
```
nasm -f elf64 -o hello.o hello.asm
```
Yukarıdaki komut, Netwide Assembler'a (NASM) "hello.asm" içindeki montaj kodundan 64 bitlik bir ELF nesne dosyası oluşturmasını söyler.
```
ld -o hello hello.o
```
Bu komut, "hello.o" nesne dosyasından "hello" adlı yürütülebilir bir dosya oluşturmak için GNU bağlayıcısını (ld) kullanır.
Uygulamamızın çalışmasını sağlayacak tüm adımları tamamladığımıza göre, aşağıdaki komutu kullanarak uygulamamızı çalıştıralım:
```
./hello
```
Bu komutu çalıştırdıktan sonra, uygulama dosyamız derlenecek ve terminal ekranına ``Hello World`` çıktısını verecektir.

> TEBRİKLER. Assembly dili giriş eğitimimizi başarıyla tamamladınız. 