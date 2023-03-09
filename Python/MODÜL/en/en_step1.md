# Modules in Python
### 1) Creating A Module
Let's create a function with our knowledge from the previous function lesson:
```python
def export(name):
    print("Hello "+ name)
```
Let's save our file and exit from the file by entering the ``wq!:`` command by pressing ``ESC`` on our keyboard, which we will use as a module.
### 2) Using A Module
In order to use the module we created above, first, let's create a new py file with the ``vim hello.py`` command. Let's integrate the module we created above onto the file we created with the ``import`` command:
 ```python
 import pythonmodules
 pythonmodules.export("Bulut Bilisimci")
```
Then, after saving and closing the file as we just showed, you can get the output by running our file with the ``python3 hello.py`` command:
```python
Hello Bulut Bilisimci
```

--> After completing the above steps, you can switch to our lesson where we will use variables on a module.