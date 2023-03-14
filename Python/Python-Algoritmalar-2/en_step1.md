Now that we have learned what the Caesar Cipher Algorithm is and how it works, we can now move on to coding our algorithm.
> First, let's create our file by using the ```vim ceaserpass.py``` command on the terminal screen.

Then write the code below into the file:
```python
def ceaserpass(message, key):
     encrypted = ''
 
     alphabet = [
         'a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm ',
         'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z '
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
-> This is the structure of our Caesar encryption algorithm. Let's move on to the next step and examine the algorithm we wrote in detail.