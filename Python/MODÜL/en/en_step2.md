### 3) Using Variables in the Module
In Python, modules contain variables as well as functions. To call these variables, it is sufficient to call the name of the module and the variable.
To test the variables in a module, let's first open the ``pythonmodules.py`` file that we use as a module with the ``vim`` command:
```python
person = {
    "name": "Bulut Bilisimci",
    "birthyear": "2023",
    "country": "Turkey"
}
```
After creating our module, let's close our file and open our ``hello.py`` command file to use the module we created:
```python
import pythonmodules
a = pythonmodules.person["year"]
print(a)
```
After writing our code to the file as above, let's first exit the file by pressing the ``ESC`` key and entering the ``wg!:`` command. You will be able to get the following output by running the file we have made with the ``python3 hello.py`` command:
```python
2023
```
--> After successfully displaying the above output, you can then proceed to the last step of our tutorial.
