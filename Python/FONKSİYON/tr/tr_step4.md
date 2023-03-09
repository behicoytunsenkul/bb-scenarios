### d) Fonksiyondan Fonksiyon Çağırma
Bazı durumlarda kullancağımız bir fonksiyonu başka bir fonksiyon içerisinde de kullanabiliyoruz:
```python
def yasHesapla(dogumYili):
    return 2023 - dogumYili
yasEda = yasHesapla(1999)
yasAli = yasHesapla(2002)
print(yasEda, yasAli)
```
Yukarıdaki ```yasHesapla``` fonksiyonunda 2 kişi için ayrı ayrı yaş hesabı yapmak yerine; tek bir fonksiyon ile 2 kişi için yaş hesabı yapabiliyoruz.

-->Yukarıdaki ```yasHesapla``` fonksiyonunu 'pythondersi.py' dosyası üzerinde denedikten sonra bu derste öğrendiklerimizi pekiştireceğimiz son adıma geçiş yapabilirsiniz.