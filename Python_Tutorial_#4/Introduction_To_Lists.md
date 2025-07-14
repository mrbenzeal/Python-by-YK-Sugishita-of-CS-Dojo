""" (Python Tutorial #4) Introduction To Lists In Python """

```python
# The lists are a type of data, just like 'strings' & 'integers'; 
# It is used to store a list of things; 
# and it's similar to 'arrays' in some other languages like 'java'.

# to define a list:

a = [3, 10, -1]

# this means assigning the list with the elements:'3, 10, -1' to the variable 'a'
```


```python
print(a)
```

    [3, 10, -1]
    


```python
# to add an item '1' to the list:

a.append(1)

# '.append()' is a predefined function used to add an item (in this case '1') to a list
```


```python
print(a)
```

    [3, 10, -1, 1]
    


```python
# One unique thing that makes Python lists different, compared to other languages, is that you can mix types in a single list. 

# A list can contain a string:

a.append("hello")
```


```python
print(a)
```

    [3, 10, -1, 1, 'hello']
    


```python
# A list can also contain another list:

a.append([1, 2])
```


```python
print(a)
```

    [3, 10, -1, 1, 'hello', [1, 2]]
    


```python
# to delete an item from the list
# eg. the last item:

a.pop()
print(a)

# '.pop()' is a predefined function used to delete an item from a list.
```

    [3, 10, -1, 1, 'hello']
    


```python
a.pop()
print(a)
```

    [3, 10, -1, 1]
    


```python
# to retrieve a specific item from the list
# note in programming, the number index starts at '0' & not at '1'.
# ie 0, 1, 2, 3, ...
# to retrieve the first item '3':

print(a[0])

# The index number of the item '3' is used to retrieve the item '3'.
# In this case, the item '3' is the first item in the list; thus, the index number '0' is used to retrieve it.
```

    3
    


```python
# or you can also use this to retrieve the first item '3':

a[0]

# This method is possible in 'jupyter notebook', but might not be feasible in 'pycham'.
```




    3




```python
# to retrieve the fourth item '1'

print(a[3])
```

    1
    


```python
# to change the content of the list
# example the first item '3' to '100'

a[0] = 100
```


```python
print(a)
```

    [100, 10, -1, 1]
    


```python
b = ["banana", "apple", "microsoft"]
```


```python
# swapping in list
# example the first item "banana" & the last item "microsoft"

temp = b[0]
b[0] = b[2]
b[2] = temp
```


```python
print(b)
```

    ['microsoft', 'apple', 'banana']
    


```python
# There is a shortcut to swapping lists:

b[0], b[2] = b[2], b[0]
```


```python
print(b)
```

    ['banana', 'apple', 'microsoft']
    


```python
# csdojo.io/python4
# csdojo.io/pat
# PyCharm, IDE
# YK from CS Dojo
```
