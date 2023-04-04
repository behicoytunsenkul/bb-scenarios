### 5- İlk Uygulamamızı Kodlayalım
Uygulamamızı kodlamaya başlamadan önce, ilk olarak dosya işlemlerini gerçekleştirebilmek için ``nano`` ve ``touch`` özelliğini kurmamız gerekiyor. Sisteminize kurulumu gerçekleştirmek için aşağıdaki komutu giriniz:
```
apk add build-base
apk add nano
apk add nasm
```
Kurulum tamamlandıktan sonra, ``clear`` komuyu ile terminal ekranımızı temizleyelim. Hazırsak, ilk uygulamamızı kodlamaya başlayalım:
İlk olarak ``nano hello.asm`` komutu ile kodlarımızı yazacağımız dosyamızı oluşturalım. Dosya ekranımız karşımıza gelecektir.
Dosyanızın içerisine aşağıdaki kodları giriniz:
```
section .data
    msg db "Helllo World"i,0
section .text
    global _start
_start:
    mov eax,4
    mov ebx,1
    mov ecx,msg
    mov edx,13
    int 0x80
    mov eax,1
    xor ebx,ebx
    int 0x80
```
Kodumuzu çalıştırma adımına geçiş yapmadan önce, yukarıda komutların ne işe yaradığını teker teker inceleyelim:
```
section .data
    msg db "Hello World",0
```
Bu kısımda, **msg** isimli bir değişken tanımladık. msg değişkeni, **db** komutu ile bir dizi byte olarak tanımlanır. Sonda yer alan 0 değeri ise dizinin sonunu belirtmektedir.
```
section .text
    global _start
_start
```
Bu kısımda, programın kod bölümü tanımlanır. **_start** etiketi, programın başlangıcını gösterir. **global** etiketi ise dışarıdan erişilebilir olmasını sağlar. 

> **_start** içerisindeki komutları incelemek için bir sonraki adıma geçiş yapınız.
