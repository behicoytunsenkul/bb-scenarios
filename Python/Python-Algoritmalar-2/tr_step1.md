Sezar Şifreleme Algoritmasının ne olduğunu ve nasıl çalıştığını öğrendiğimize göre, artık algoritmammızı kodlama aşamasına geçebiliriz. 
> İlk olarak terminal ekranı üzerinde ```vim ceaserpass.py``` komutunu kullanarak dosyamızı oluşturalım.

Sonrasında aşağıda yer alan kodu, dosyanın içerisine yazınız: 
```python
def ceaserpass(message, key):
    encrypted = ''
 
    alphabet = [
        'a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm',
        'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z'
    ]
    for i in message:
 
        if i not in alphabet:
            encrypted += i
        else:
            encrypted += alphabet[
                (alphabet.index(i)+key) % len(alphabet)]
 
    print("Encrypted message is: ", encrypted)
 
 
key = int(input('Key value: '))
 
text = input("Message: ")
ceaserpass(text, key)
```
-> Sezar şifreleme algoritmamımızın yapısı bu şekildedir. Bir sonraki adıma geçerek, yazdığımız algoritmayı detaylı bir şekilde inceleyelim.