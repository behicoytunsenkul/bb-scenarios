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
