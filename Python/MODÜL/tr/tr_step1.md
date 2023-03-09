# Python Modüller
### 1) Modül Oluşturmak
Bir önceki fonksiyon dersindeki bilgilerimiz ile bir fonksiyon oluşturalım:
```python
def export(name):
    print("Hello "+ name)
```
Modül olarak kullanacağımız fonksiyonumuzu klavyemiz üzerinden ``ESC`` basarak ``wq!:`` komutunu girerek dosyamızı kaydedip, dosyadan çıkış yapalım.
### 2) Modülü Kullanmak
 Yukarıda oluşturmuş olduğumuz modülü, kullanabilmemiz için ilk olarak ``vim hello.py`` komutu ile yeni bir py uzantılı bir dosya oluşturalım. Oluşturduğumuz dosya üzerine yukarıda oluşturduğumuz modülü, ```import``` komutu ile entegre edelim:
 ```python
 import pythonmodules
 pythonmodules.export("Bulut Bilisimci")
```
Ardından dosyayı az önce gösterdiğimiz gibi kaydedip, kapattıktan sonra ``python3 hello.py`` komutu ile dosyamızı çalıştırarak çıktıyı elde edebilirsiniz:
```python
Hello Bulut Bilisimci
```

--> Yukarıdaki adımları tamamladıktan sonra, bir modül üzerinde değişkenleri kullanacağımız dersimize geçiş yapabilirsiniz.