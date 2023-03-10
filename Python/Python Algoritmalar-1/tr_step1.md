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
3. Since we will draw our pyramid using rows and columns, we define 2 for loops that will be nested. With the formula ```(x-i)+1``` used in the second for loop, the necessary spaces are created for each line; The variable ```i``` is the current row number.
4. The formula ```2*i-1``` in the ``while`` loop allows adding the asterisk for each position where the row value is i.

>In this step of our training, we learned the algorithm logic at a basic level by drawing a pyramid. In our next step, we will ask you to develop an algorithm based on the desired output.