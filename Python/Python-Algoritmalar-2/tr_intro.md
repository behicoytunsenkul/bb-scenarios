## Python Algoritmalar-2
Python Algoritmalar-2 eğitimimize hoşgeldiniz. Bu eğitimimizde Pyton Algoritmalar-1 eğitimimizdeki gibi, orta seviye zorluktaki bir örneği inceleyeceğiz. Bu dersimizdeki örneğimizin konusu, Python ile Sezar Şifreleme algoritmasının nasıl yazılacağıdır.
Algoritmamızın kodlmasına geçmeden önce Sezar Şifreleme Algoritmas'nın ne olduğunu ve nasıl çalıştığını inceleyelim:

### 🔒Sezar Şifreleme Algoritması Nedir?
Sezar Şifreleme, tarihte bilinen ilk şifreleme tekniği olarak geçmektedir. Sezar Şifreleme, adından da anlaşıldığı gibi ilk olarak Jul Sezar tarafından kullanılmıştır. Kullanım amacı ise savaş zamanlarında gönderilen mesajların düşman tarafından ele geçirildiğinde okunmasını engellemektir. 

### Sezar Şifreleme Algoritması Nasıl Çalışır?
Oldukça basit bir yöntem olan Sezar Şifreleme Algoritması, belirlenen anahtar değere göre harfleri kaydırarak oluşturulmaktadır.  Ufak bir örnek yaparak, Sezar Şifreleme Algoritmasının çalışma mantığına bakalım:
Şifrelemek istediğimiz kelime ***yazılım*** olsun. Anahtar değerimiz yani harf kaydırma değerimiz ise 2 olsun. Şimdi bu bilgileri kullanarak, kelimemizi şifreleyelim:
Y -> A
A -> C
Z -> B
I -> J
L -> N
I -> J
M -> O
İşlemlerimizin sonucunda şifrelenmiş kelimemiz **acbjnjo** olarak karşımıza çıkmaktadır.

> Bir sonraki adımımızda Python'da Sezar Şifreleme Algoritmasının nasıl oluşturulacağını öğreneceğiz.


