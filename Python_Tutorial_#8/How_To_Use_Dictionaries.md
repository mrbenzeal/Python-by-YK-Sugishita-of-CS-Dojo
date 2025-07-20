```python
# What are Dictionaries in Python?
# Dictionaries in Python are data structures that store key-value pairs, allowing for efficient data retrieval based on unique keys.
# This is sort of like a look-up table
# It can sometimes be referred to as key-value pairs, e.g, in a predefined dictionary: d = {"George": 24, "Tom": 32};
# where the key is some unique identifier, while the value is something we associate with that key.

# How do you create an empty dictionary in Python?
# To create an empty dictionary, we can write: d = dict() or as below 

d = {}

# The above defines an empty dictionary.
```


```python
# How to add keys and values to an empty dictionary?
# After defining an empty dictionary, we can add the key-value pairs as follows:

d["George"] = 24
d["Tom"] = 32
d["Jenny"] = 16
```


```python
# To find a value associated with a certain key, e.g, George, we used the print function below:

print(d["George"])
```

    24
    


```python
# To also find a value associated with the key, e.g, Tom, we used the print function below:

print(d["Tom"])
```

    32
    


```python
# When we try to find a value associated with a certain key that does not exist in the dictionary, e.g, Alice, 
# We will get the error message.

print(d["Alice"])
```


    ---------------------------------------------------------------------------

    KeyError                                  Traceback (most recent call last)

    <ipython-input-6-e722e03f8739> in <module>()
    ----> 1 print(d["Alice"])
    

    KeyError: 'Alice'



```python
print(d["Jenny"])
```

    16
    


```python
# As we can see above, the value associated with the key "Jenny" was 16,
# We can change the value associated with the key "Jenny" as follows:

d["Jenny"] = 20
```


```python
# When we print the key "Jenny", we find out that its value has changed from "16" to "20".

print(d["Jenny"])
```

    20
    


```python
# Note: while the values can be of any type, keys are commonly strings or numbers.

d[10] = 100
```


```python
print(d[10])
```

    100
    


```python
# how to iterate over key-value pairs?

for key, value in d.items():
    print("key:")
    print(key)
    print("value:")
    print(value)
    print("") # empty line for better readability
```

    key:
    George
    value:
    24
    
    key:
    Tom
    value:
    32
    
    key:
    Jenny
    value:
    20
    
    key:
    10
    value:
    100
    
    


```python

```
