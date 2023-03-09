### Function Example
**Using Functions in Python** In the last step of our course, we will reinforce what we have learned throughout the course through the example below:

First of all, we define our ``retireCalc`` function and operations that we want to take place in the function.
```python
def ageCalc(birthDay):
    return 2023 - birthDay
def retireCalc(birthDay, name):
    age = ageCalc(birthDay)
    retire = 65 - age
    if retire > 0:
        print(name+' you will retire after {retire} years')
    else:
        print('You are already retired')
```
As you can see above, we have defined 2 different functions as we need to account for the first person in order to make a pension account. Now, to run our function, we need to enter the code below:
```python
retireCalc(1983,'Ali')
```
After logging in the code that will allow us to run our function, you will run a screen output like the following by running our 'pythondersi.py' file through the terminal:
```python
Ali you will retire after 34 years
```

--> As you can see, it is so easy to use functions in the Python language. ** Functions ** As in the examples you have seen during the course, ** provide simplicity in terms of time and complexity in our daily operations.
