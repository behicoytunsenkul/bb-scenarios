Fonksiyonumuzu tanımladıktan sonra ```encrypted``` isimli, şifrelenmiş mesajı eşitleyeceğimiz değişkenimizi oluşturuyoruz. Sonrasında şifrelemede kullanacağımız alfabeyi, ```alphabet``` değişkeni ile dizi şeklinde tanımlıyoruz.
Değişkenlerimizi tanımladıktan sonra,
```python
for i in message:
    if i not i in alphabet:
        encrypted +=i
    else:
        encrypted += alphabet[(alphabet.index(i)+key) % len(alphabet)]
```
Alınan mesajı, şifrelemek için her bir harfi üzerinde bir işlem yapmamız gerekiyor. Bunun içinde ```for``` döngüsü tanımlıyoruz. Sonrasında döngü içerisinde ```if-else``` yapısını kullanarak mesaj içerisindeki karakterlerin alfabe elemanları ile eşleşip eşleşmediğini kontrol ediyoruz. Eğer alfabenin içinden bir eleman değilse, değişime uğramadan ilgili harfi çıktıya veriyoruz. Ancak ilgili harf, alfabenin içerisinde ise ilgili harfin key değeri kadar sonrasındaki harfi alarak yeni şifre olarak çıktı veriyor ve bu şekilde metin tamamen şifreli hale getirilene kadar işlemler devam ettiriliyor.
> Bir sonraki adıma geçerek, oluşturmuş olduğumuz algoritmayı bir örnek ile test ederek sonuçlarını inceleyeceğiz.