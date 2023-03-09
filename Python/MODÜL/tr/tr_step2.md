### 3) Modüldeki Değişkenleri Kullanmak
Python'da modüller fonksiyonların yanı sıra değişkenler de içerir. Bu değişkenleri çağırmak için modülün ve değişkenin adını çağırmak yeterlidir.
Bir modül içerisinde değişkenleri denemek için ilk olarak modül olarak kullandığımız ``pythonmodules.py`` dosyasını ``vim`` komutu ile açalım:
```python
person = {
    "name": "Bulut Bilisimci",
    "birthyear": "2023",
    "country": "Turkey"
}
```
Modülümüzü oluşturduktan sonra dosyamızı kapatarak, oluşturduğumuz modülü kullanmak için ``hello.py`` komutu dosyamızı açalım:
```python
import pythonmodules
a = pythonmodules.person["year"]
print(a)
```
Yukarıdaki gibi kodumuzu dosyaya yazdıktan sonra, ilk önce ``ESC`` tuşuna basıp ``wg!:`` komutunu girerek dosyadan çıkış yapalım. Yapmış olduğumuz dosyayı ``python3 hello.py`` komutu ile çalıştırarak aşağıdaki çıktıyı elde edebileceksiniz:
```python
2023
```

--> Başarılı bir şekilde yukarıdaki çıktıyı görüntüledikten sonra bir sonra, eğitimimizin son adımına geçiş yapabilirsiniz.