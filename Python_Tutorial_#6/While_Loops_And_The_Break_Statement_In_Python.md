""" (Python Tutorial #6) While Loops and The Break Statement in Python """

```python
# Recapping the previous 'for loop' example of range(1, 5) = range(5) or total = list(range(1, 5)) = [1,2,3,4]

total = 0 # initialising the variable 'total' to '0'.
for i in range(1, 5): # note: the index 'i' is automatically initialised to '0' in 'for loop' and will go through the list.
    total += i
print(total)
```

    10
    


```python
# Now let's use a 'while loop' for the same example

total2 = 0 # initializing the variable 'total2' to '0'
j = 1 # initialising the index 'j' to '1'. The index is not initialised in the 'while loop' like in the 'for loop'; thus, we're to initialise it by ourselves.
while j < 5:
    total2 += j
    j += 1 # increment 'j'
print(total2)
```

    10
    


```python
# 'while loop' is useful in a case when we don't know how many loops we need beforehand

given_list = [5, 4, 4, 3, 1,-2,-3,-5]
# If we are to find the sum of only the positive numbers

total3 = 0
i = 0 
while given_list[i] > 0:
    total3 += given_list[i]
    i += 1 # increment 'i'
print(total3)

# note: this method is only possible if we have at least one negative number in the list.
```

    17
    


```python
# If we omit or pop all the negative elements of the given list and try using the same condition
# We will get a 'list index out of range' index error from Python
# This is because when the index is increased to '5', which is also greater than '0', but nothing exists at index '5' in the list,
# Python will indicate a 'list index out of range' index error 

given_list = [5, 4, 4, 3, 1]

total3 = 0
i = 0
while given_list[i] > 0:
    total3 += given_list[i]
    i += 1
print(total3)
```


    ---------------------------------------------------------------------------

    IndexError                                Traceback (most recent call last)

    C:\Users\MRBENZ~1\AppData\Local\Temp/ipykernel_5724/634915877.py in <module>
          8 total3 = 0
          9 i = 0
    ---> 10 while given_list[i] > 0:
         11     total3 += given_list[i]
         12     i += 1
    

    IndexError: list index out of range



```python
# We can fix this index error by including an extra condition in the 'while loop'
# i.e i < 5 or i < len(given_list)

given_list = [5, 4, 4, 3, 1]

total3 = 0
i = 0
while i < len(given_list) and given_list[i] > 0:
    total3 += given_list[i]
    i += 1
print(total3)
```

    17
    


```python
# We can also find the sum of only the positive numbers using a 'for loop' and the 'break statement'

given_list2 = [5, 4, 4, 3, 1, -2, -3, -5]
total4 = 0
for element in given_list2:
    if element <= 0:
        break
    total4 += element
print(total4)
```

    17
    


```python
# We can also find the sum of only the positive numbers using a 'while loop' and the 'break statement' 

given_list2 = [5, 4, 4, 3, 1, -2, -3, -5]
total5 = 0
i = 0
while True: # here we choose something always true, like 'while 1 < 2' or just 'while True' because either of these two statements is always true
    total5 += given_list2[i]
    i += 1
    if given_list2[i] <= 0:
        break
print(total5)
```

    17
    


```python
given_list3 = [7, 5, 4, 4, 3, 1, -2, -3, -5, -7]

# csdojo.io/python6
# follow CS Dojo on Facebook
```
