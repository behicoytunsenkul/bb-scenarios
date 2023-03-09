### d) Function Calling From Function
In some cases, we can use a function in another function:
```python
def ageCalc(birthYear):
    return 2023 - birthYear
ageEda = ageCalc(1999)
ageAli = ageCalc(2002)
print(ageEda, ageAli)
```
In the ``ageCalc`` function above, instead of taking into account the age of 2 people; With a single function, we can age 2 people.

--> After completing the above, you can switch to the last step that we will reinforce what we have learned in this course.sss