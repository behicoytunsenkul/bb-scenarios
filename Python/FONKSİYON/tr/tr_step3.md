### c) Fonksiyondan Geriye Bilgi Gönderme
Fonksiyon içerisinde ```print()``` ile bilgi yazdırmak yerine bilgiyi geriye de döndürebiliyoruz.
```python
def hello(name):
    return "Merhaba" + name
print(hello(" Bulut Bilisimci")
```
Yukarıda gördüğünüz gibi print ile bilgiyi foksiyon içerisinde yazdırmak yerine 'Merhaba Bulut Bilisimci' bilgisini fonksiyondan geriye ```return``` komutu ile geri döndürerek, yazıyı çıktı olarak ekrana verdik.