""" (Python Tutorial #1) Python Tutorial for Absolute Beginners - What Are Variables """

```python
# NB: anything after the '#' sign is called 'comment' in Python,
# In Python, it is not executed but used to explain or comment on our code

# to print a string, eg, "Hello World"

print("Hello World")
```

    Hello World
    


```python
# You can also use a single quote, eg, 'more string'

print('more string')
```

    more string
    


```python
# You can also print a number or an integer, eg, '3'

print(3)

# note that there is no single or double quote around the number '3'
# This is because '3' is not a string, but an integer or number.
```

    3
    


```python
# You can also print multiple lines within the same cell:

print('more string') 
print(3)
```

    more string
    3
    


```python
# What are variables?

a = 1

# This means assign the value '1' to the variable named 'a'.
# In other languages like C or C++, 'a' is like a box which contains the value '1'
# but in Python; this means the variable 'a' refers to the value '1'
```


```python
print(a)

# note that there is no single or double quote around the character 'a'.
# This is because 'a' is not a string, but a variable.
```

    1
    


```python
b = 2
```


```python
print(b)
```

    2
    


```python
print(a)
print(b)
```

    1
    2
    


```python
# You can also assign a string to a variable

c = ("hello there")
```


```python
print(c)
```

    hello there
    


```python
# note earlier we had b = 2

print(b)
```

    2
    


```python
# You can also reassign a value to a variable

b = 1
```


```python
# 'b' will now refer to the value '1'

print(b)
```

    1
    


```python
# What happens if you try printing a variable that does not exist yet?

print(e)
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    C:\Users\MRBENZ~1\AppData\Local\Temp/ipykernel_5544/4007279472.py in <module>
    ----> 1 print(e)
    

    NameError: name 'e' is not defined



```python
# to fix this

e = "this is a string"
```


```python
print(e)
```

    this is a string
    


```python
# Is it possible to assign a variable to another variable?
# Yes is the answer

print(a)
print(c)
```

    1
    hello there
    


```python
# assigning a variable to another variable

f = a

# This means that the variable 'f' is now referring to the value the variable 'a' is referring to, ie '1'
# thus, the variables 'a' & 'f' are now referring to the value '1'
# The variable 'f' doesn't refer to the variable 'a' but its value '1'
```


```python
print(f)
```

    1
    


```python
# When you reassign a new value to the variable 'a'.

a = 2

# it stops referring to its old value '1', but starts referring to the new value '2'
```


```python
print(a)
```

    2
    


```python
# while the variable 'f' continues to stay & refers to  the value '1'

print(f)
```

    1
    


```python

```
