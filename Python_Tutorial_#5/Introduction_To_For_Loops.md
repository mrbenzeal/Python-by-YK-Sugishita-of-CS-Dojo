""" (Python Tutorial #5) Introduction to For Loops in Python """

```python
# Suppose you have this list

a = ["banana", "apple", "microsoft"]
```


```python
# to iterate through each element of the list, ie, to do something with each item of the list
# one way to do that is:

print(a[0])
print(a[1])
print(a[2])
```

    banana
    apple
    microsoft
    


```python
# The aforementioned method becomes cumbersome because of repeating the statement all over again.
# It will be a lot of work, eg, if the list has 100 elements.
# This is where the 'for loop' comes in, eg:

for element in a:
    print(element)
    
# The whole block says, for each element or item in 'a'(the list), do the following (in this case, printing the elements)
```

    banana
    apple
    microsoft
    


```python
# You can have multiple statements in the 'for block' as well

for element in a:
    print(element)
    print(element)
```

    banana
    banana
    apple
    apple
    microsoft
    microsoft
    


```python
# another example

b = [20, 10, 5]
for e in b:
    print(e)
    
# The word 'element' or 'item' used in other previous examples is something we can choose.
# We can use pretty much anything we want; thus, in this case, we are using the letter 'e'.
```

    20
    10
    5
    


```python
# to find the sum of the list
# We first initialise a new variable called 'total' & initialise it to '0'.

b = [20, 10, 5]
total = 0
for e in b:
    total = total + e
print(total)    

# the 'for block' will go via each element in 'b'; thus 'e' will be initially '20', then '10' & then '5'
# then for each 'e', we are going to add it to the initialised total (ie, 0 + 20 + 10 + 5 = 35)
# thus, when we print 'total', we get '35'
```

    35
    


```python
# The usefulness of the range function in Python
# if we want to find the sum of, eg, 1, 2, 3, 4

range(1, 5)

# this means create a range of numbers starting at '1' through '5' BUT not including '5'
# then putting it into a list function to convert it into a list

list(range(1, 5))

# Let's now put it into a new variable 'c'

c = list(range(1, 5))

# and then print what's inside 'c'

print(c)

# This method is better in the case of finding the sum of numbers ranging from '1' to '100'
```

    [1, 2, 3, 4]
    


```python
# You can use this range function in a 'for loop'

for i in range(1, 5):
    print(i)
```

    1
    2
    3
    4
    


```python
# to find the sum of the aforementioned numbers

total2 = 0
for i in range(1, 5):
    total2 = total2 + i
print(total2)
```

    10
    


```python
# or total2 += i

total2 = 0
for i in range(1, 5):
    total2 += i

# This says the new value of 'total2' should be the sum of the old value of 'total2' plus 'i'.

print(total2)
```

    10
    


```python
# another example

print(list(range(1, 8)))
```

    [1, 2, 3, 4, 5, 6, 7]
    


```python
# What if we wish to find the sum of only multiples of '3' in the aforestated list
# First we need to know what is called the 'modulo operator'
# eg. '%'

print(5 % 3)
print(4 % 3)
print(1 % 3)
print(2 % 3)
print(6 % 3)
print(3 % 3)
print(7 % 3)

# to check if a number is a multiple of another number, we use the 'modulo ,operator' eg, '%'
# this means, to divide a number 'a' by another number 'b' (divisor) & stating the remainder of the solution
# if the remainder is equal to '0', then this implies that the number 'a' is a multiple of the number 'b' (divisor).
```

    2
    1
    1
    2
    0
    0
    1
    


```python
# now to find the sum of only multiples of '3' in the aforestated list

total3 = 0
for i in range(1, 8):
    if i % 3 == 0:
        total3 += i
print(total3)

# the 'if block' inside the 'for block' implies checking if 'i' is a multiple of '3' (ie, remainder = 0);
# and if that's true, then add 'i' to the 'total3'.
# note range(1, 8) is [1, 2, 3, 4, 5, 6, 7]; the multiples of '3' are '3' & '6'; and when we add 3 + 6 = 9.
```

    9
    


```python
# Can you compute all multiples of 3 & 5 that are less than 100?

print(list(range(1, 100)))
```

    [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 58, 59, 60, 61, 62, 63, 64, 65, 66, 67, 68, 69, 70, 71, 72, 73, 74, 75, 76, 77, 78, 79, 80, 81, 82, 83, 84, 85, 86, 87, 88, 89, 90, 91, 92, 93, 94, 95, 96, 97, 98, 99]
    


```python

```
