""" (Python Tutorial #7) More About For Loops in Python & Solutions to the Last 2 Problems """

```python
# note: In a recapping of previous tutorials on 'for loops', 
# if we have a variable 'a' equal to a list with three elements of 'apple', 'banana' and 'republic'

a = ["apple", "banana", "republic"]
```


```python
# we can print each element in the list with:

for element in a:
    print(element)
```

    apple
    banana
    republic
    


```python
# another way of doing the same thing is by using the indexes, or the indices of the three elements.

for i in range(0, 3): # or range(3) or range(len(a)), which means the indexes '0', '1', '2', but not including the index '3'.
    print(a[i])
```

    apple
    banana
    republic
    


```python
# why would we want to use the second method instead of the first?
# this is because in some cases the index matters and not just the elements.
# for example, if we which to print 'apple' once, 'banana' twice, and 'republic' three times.

for i in range(len(a)):
    for j in range(i + 1): # note that the value of 'j' does not matter because we are not going to use it. the important thing is that we going to go through the inner 'for loop'.
        # i = 0 -> j = 0 {i.e., 'j' once when 'i' is equal to '0'}
        # i = 1 -> j = 0, 1 {i.e., 'j' twice when 'i' is equal to '1'}
        # i = 2 -> j = 0, 1, 2 {i.e., 'j' three times when 'i' is equal to '2'}
        print(a[i]) # so within this 'for loop', within the outer 'for loop', we can now print.
        
```

    apple
    banana
    banana
    republic
    republic
    republic
    


```python
# Tutorial 5
# Can you compute the sum of all multiples
# of 3 and 5 that are less than 100?
print(list(range(1, 100)))
```

    [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 58, 59, 60, 61, 62, 63, 64, 65, 66, 67, 68, 69, 70, 71, 72, 73, 74, 75, 76, 77, 78, 79, 80, 81, 82, 83, 84, 85, 86, 87, 88, 89, 90, 91, 92, 93, 94, 95, 96, 97, 98, 99]
    


```python
# here is the solution 

total = 0 # first initializing 'total' to '0'
for i in range(1, 100):
    if i % 3 == 0: 
        total += i
    elif i % 5 == 0:
        total += i
print(total)
```

    2318
    


```python
# Tutorial 6
# given the below list with the assumption that we don't necessarily know the content or the length of the list
# but we know that it's sorted in a descending order so that the largest number comes first 
# and then you go right, the number always stays the same or go down.
# And we assume that there is at least one positve number in the list
# And we wish to find the sum of only the negative numbers there.

given_list = [7, 5, 4, 4, 3, 1, -2, -3, -5, -7]

total2 = 0 # first initializing 'total2' to '0'
j = len(given_list) - 1 # and initializing an index, let's say 'j' to 'len(given_list) - 1'
while given_list[j] < 0: # changing 'j' so that we can iterate over only the negative numbers, starting from the right (just incase there are large positive numbers in the list) 
    total2 += given_list[j]
    j -= 1 # this is decreasing 'j' by one
print(total2)
```

    -17
    


```python
# sorry..
# don't want to wait for the next tutorial?
# I'd recommend my courses on Lynda.com and Pluralsight
# - Lynda.com: Get Ready for Your Coding Interview
# - Pluralsight: Introduction to Data Visualization with Python
# (you can take these for free)
# Links in the description below

# more YouTube tutorials coming up, too!
```
