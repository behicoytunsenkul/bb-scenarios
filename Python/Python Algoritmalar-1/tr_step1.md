## Python Algoritmalar: Piramit Çizme
Python Algoritmalar-1 dersimizin bu adımında, * sembolünü kullanarak ve kullanıcıdan alınan satır değerine göre piramit çizen bir algoritma yazacağız. İlk olarak kodumuzu, oluşturduğumuz pythonalgorithm.py dosyasına yazalım ve sonrasında kodun nasıl çalıştığını detaylı bir şekilde inceleyelim:
```python
x = int(input("Enter the number of row: "))
def pyramid(x):
    k=0
    for i in range(1,x+1):
        for j in range(1,(x-i)+1):
            print(end=" ")
        while k!=(2*i-1):
            print("*",end="")
            k+=1
        k=0
        print()
pyramid(x)
```
### Kodun Çalışma Mantığı
1. İlk olarak ```input``` komutunu kullanarak, satır değerini almak iiçin bir x değişkeni tanımlayarak kullanıcdan istediği değeri alıyoruz.
2. Piramit şeklinin çizilmesini sağlayacak fonksiyonumuzu ```def``` komutu ile tanımlıyoruz.
3. Satır ve sütunları kullanarak piramidimizi çizeceğimiz için iç içe olacak 2 adet for döngüsü tanımlıyoruz. İkinci for döngüsünde kullanılan ``(x-i)+1`` formülü ile her satır için gerekli boşluklar oluşturulur; ```i``` değişkeni geçerli satır numarasıdır.
4. "while" döngüsündeki ```2*i-1``` formülü, satır değerinin i olduğu her konum için yıldız eklenmesine izin verir.

>Eğitimimizin bu adımında bir piramit çizerek algoritma mantığını temel düzeyde öğrendik. Bir sonraki adımda, sizden istenen çıktıya dayalı bir algoritma geliştirmenizi isteyeceğiz.