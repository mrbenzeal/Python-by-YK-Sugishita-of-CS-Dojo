""" (Python Tutorial #3) How To Use Functions In Python """

```python
# What are functions?
# a collection of instructions
# a collection of code

def function1():
    print("ahhhh")
    print("ahhhhh 2")
print("this is outside the function")
```

    this is outside the function
    


```python
# Noted: the two lines under the function clause 'def function1()' was not printed in the previous cell.
# Only the line outside the function clause was printed ie 'print("this is outside the function")'
# To call or use the function 'def function1()' and print the lines under it, we do this:

function1()
```

    ahhhh
    ahhhhh 2
    


```python
function1()
function1()
```

    ahhhh
    ahhhhh 2
    ahhhh
    ahhhhh 2
    


```python
# a mapping
# input or an argument

def function2(x):
    return 2*x

# This means define a function called 'function2' that will take an input or argument called 'x'
# And in return to whoever call this function, it will return an output called '2*x'
```


```python
# Now to use or call the aforementioned function:

a = function2(3)

# return value or output
```


```python
print(a)
```

    6
    


```python
b = function2(4)
```


```python
print(b)
```

    8
    


```python
c = function2(5)
print(c)
```

    10
    


```python
# What if we try calling the function without an argument:

d = function2()
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    <ipython-input-10-fb94927463a6> in <module>()
    ----> 1 d = function2()
    

    TypeError: function2() missing 1 required positional argument: 'x'



```python
# An example of a single function with multiple arguments:

def function3(x, y):
    return x + y
```


```python
e = function3(1, 2)
print(e)
```

    3
    


```python
# To combine a function as a collection of code and a mapping:

def function4(x):
    print(x)
    print("still in this function")
    return 3*x
```


```python
f = function4(4)
```

    4
    still in this function
    


```python
print(f)
```

    12
    


```python
def function5(some_argument):
    print(some_argument)
    print("weeee")
    
# Note here, we do not have any Return value.
```


```python
function5(4)
```

    4
    weeee
    


```python
# BMI calculator

name1 = "Obinna"
height_m1 = 2
weight_kg1 = 90

name2 = "Obinna's sister"
height_m2 = 1.8
weight_kg2 = 70

name3 = "Obinna's brother"
height_m3 = 2.5
weight_kg3 = 160
```


```python
# Using functions to calculate the BMI for each person, and to determine if each person is overweight or not. 

def bmi_calculator(name, height_m, weight_kg):
    bmi = weight_kg / (height_m ** 2)
    print("bmi: ")
    print(bmi)
    if bmi < 25:
        return name + " is not overweight"
    else:
        return name + " is overweight"
```


```python
result1 = bmi_calculator(name1, height_m1, weight_kg1)
result2 = bmi_calculator(name2, height_m2, weight_kg2)
result3 = bmi_calculator(name3, height_m3, weight_kg3)
```

    bmi: 
    22.5
    bmi: 
    21.604938271604937
    bmi: 
    25.6
    


```python
print(result1)
print(result2)
print(result3)
```

    Obinna is not overweight
    Obinna's sister is not overweight
    Obinna's brother is overweight
    


```python
# Solution to a given task: 
# The following function converts miles to kilometers.
# Returning an output of km = 1.6 * miles.
# Note: 1 mile = 1.6 km.

def convert(miles):
    return 1.6 * miles
```


```python
print(convert(1))
```

    1.6
    


```python
print(convert(2))
```

    3.2
    


```python
# csdojo.io/python3
# csdojo.io/news - 2-4
# YK from CS Dojo
```
