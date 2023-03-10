## Python Algorithms: Pyramid Drawing
In this step of our Python Algorithms-1 lesson, we will write an algorithm that draws a pyramid using the * symbol and based on the row value received from the user. First, let's write our code in the pythonalgorithm.py file we created, and then let's examine in detail how the code works:
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
### Working Logic of the Code
1. First, using the ```input``` command, we define an x variable to get the row value and get the desired value from the user.
2. We define our function that will draw the pyramid shape with the ``def``` command.
3. Since we will draw our pyramid using rows and columns, we define 2 for loops that will be nested. With the formula ```(x-i)+1``` used in the second for loop, the necessary spaces are created for each line; The variable ```i``` is the current row number.
4. The formula ```2*i-1``` in the ``while`` loop allows adding the asterisk for each position where the row value is i.

>In this step of our training, we learned the algorithm logic at a basic level by drawing a pyramid. In our next step, we will ask you to develop an algorithm based on the desired output.