### Pekiştirme Örneği
**Python'da Fonksiyonları Kullanma** dersimizin son adımında ders boyunca öğrendiklerimizi, aşaağıdaki örnek üzerinden pekiştireceğiz:

İlk olarak ```EmeklilikSayaci``` fonksiyonumuzu ve fonksiyon içerisinde gerçekleşmesini istediğimiz işlemleri tanımlıyoruz.
```python
def yasHesapla(dogumYili):
    return 2023 - dogumYili
def EmeklilikSayaci(dogumYili, isim):
    yas = yasHesapla(dogumYili)
    emeklilik = 65 - yas
    if emeklilik > 0:
        print(isim+' emekliliginize {emeklilik} yil kaldi')
    else:
        print('Zaten emeklisiniz')
```
Yukarıda gördüğünüz gibi emeklilik hesabını yapabilmemiz için ilk olarak kisinin yas hesabını yapmamız gerektiğinden 2 farklı fonksiyon tanımladık. Şimdi ise fonksiyonumuzu çalıştırmak için aşağıdaki kodu dosyamıza girmemiz gerekiyor:
```python
EmeklilikSayaci(1983,'Ali')
```
Fonksiyonumuzu çalıştırmamızı sağlayacak kodu giriş yaptıktan sonra terminal üzerinden 'pythondersi.py' dosyamızı çalıştırarak aşağıdaki gibi bir ekran çıktısı elde edeceksiniz:
```python
Ali emekliliginize 34 yil kaldi
```

--> Gördüğünüz gibi Python dilinde fonksiyonları kullanmak işte bu kadar kolay. Ders boyunca görmüş olduğunuz örneklerde olduğu gibi **Fonksiyonlar** günlük işlemlerimizde zaman ve karmaşıklık açısından basitlik sağlamaktadır.
