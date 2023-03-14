After defining our function, we create our variable named ``encrypted``` with which we will synchronize the encrypted message. Then we define the alphabet that we will use in encryption as a string with the variable ``alphabet```.
After defining our variables,
```python
for i in message:
     if i not i in alphabet:
         encrypted +=i
     else:
         encrypted += alphabet[(alphabet.index(i)+key) % len(alphabet)]
```
In order to encrypt the received message, we need to perform an operation on each letter. In this we define a ``for`` loop. Then, we check whether the characters in the message match the alphabet elements by using the ``if-else`` structure inside the loop. If it is not an element of the alphabet, we output the corresponding letter without any changes. However, if the relevant letter is in the alphabet, it takes the letter after the key value of the relevant letter and outputs it as a new password, and in this way, the operations are continued until the text is completely encrypted.
> Moving on to the next step, we will test the algorithm we have created with an example and examine the results.