""" (Python Tutorial #2) How to Use If Else Statements in Python """

```python
# dealing with one case of the 'if clause'. 

a = 1
b = 2
if a < b:
    print("a is less than b")
    print("a is definitely less than b")
print("Not sure if a is less than b")

# the whole two lines under 'if a < b:'; print("a is less than b") & print("a is definitely not less than b") is called an 'if clause'.
# Python knows that because of the colon sign ':' after the 'b' & the four spaces before the 'print()'.
# they are all inside the 'if block' & can only be exercuted only if the 'if clause' is valid. 
# but the line 'print("Not sure if a is less than b")' is outside the 'if block', thus not influenced by the 'if clause'.
```

    a is less than b
    a is definitely less than b
    Not sure if a is less than b
    


```python
# dealing with two cases; eg. conbining the 'if clause' & the 'else clause'.

c = 5
d = 4
if c < d:
    print("c is less than d")
else:    
    print("c is NOT less than d")
    print("I don't think c is less than d")
print("outside the if or else blocks")

# any of the lines inside the 'if or else blocks' can only be exercuted only if either the 'if or else clause' is valid.
```

    c is NOT less than d
    I don't think c is less than d
    outside the if or else blocks
    


```python
# dealing with three or more cases; eg. conbining the 'if clause', the 'elif clause' & the 'else clause'.
# NB: in python & other programming languages, the single equality sign '=' is an assignment operator; 
# ie. assigning what is on the right hand side to the left hand side.
# while the double equality sign '==' is the evaluation operator (equal to); ie. checking if two variables are are equal.

e = 20
f = 8
if e < f:
    print("e is less than f")
elif e == f:
    print("e is equal to f")
elif e > f + 10:
    print("e is greater than f by more than 10")    
else:    
    print("e is greater than f")
    
# note: we could have multiple 'elif clauses'.
```

    e is greater than f by more than 10
    


```python
# another way of dealing with three or more cases without using the 'elif clause'.

g = 9
h = 8
if g < h:
    print("g is less than h")
else:
    if g == h:
        print("g is equal to h")
    else:
        print("g is greater than h")
```

    g is greater than h
    


```python
# creating a BMI (a number that can tell if a person is over weight or not, depending on their height & weight) calculator. 

name = "Benzeal"
height_m = 2
weight_kg = 110

bmi = weight_kg / (height_m ** 2)
if bmi < 25:
    print(name)
    print("is not overweight")
else:
    print(name)
    print("is overweight")
print("bmi: ")
print(bmi)
```

    Benzeal
    is overweight
    bmi: 
    27.5
    


```python
# csdojo.io/python2
# csdojo.io/pat
# YK from CS Dojo
```
