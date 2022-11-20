# Learning Python

## Cool Features

### Function Attributes

```python
def func(x):
    intermediate_var = x**2 + x + 1

    if intermediate_var % 2:
        y = intermediate_var ** 3
    else:
        y = intermediate_var **3 + 1

    # setting attributes here
    func.optional_return = intermediate_var
    func.is_awesome = 'Yes, my function is awesome.'

    return y

y = func(3)
print('Final answer is', y)
print('Show calculations -->', func.optional_return)
print('Is my function awesome? -->', func.is_awesome)
# Accessing function attributes
```

### For-else loop

```python
my_list = ['some', 'list', 'containing', 'five', 'elements']

min_len = 3

for element in my_list:
    if len(element) < min_len:
        print(f'Caught an element shorter than {min_len} letters')
        break
else:
    print(f'All elements at least {min_len} letters long')
```

### Separators for ‘int’

```python
a = 3250
b = 67_543_423_778 + 1
c = 6_7_5_43_423_7_7_8 + 1

print(type(a))
print(type(b))

print(a)
print(b)
```

### eval() and exec()

```python
a = 3
# c = 0
b = eval('2 + a')

exec('c = a + b')

print(a)
print(b)
print(c)
```

### Ellipsis

```python
def foo():
    pass


def foo2():
    ...

###############################
###############################

def foo3(m=...):
    if m is ...:
        print(type(m))
        print('nothing received')
    elif m is None:
        print('None')
    else:
        print(type(m))
        print('another typy')


foo3()

###############################
###############################

import numpy as np

a = np.arange(16).reshape((2, 2, 2, 2))

print(a)
print(a[..., 0].flatten())
print(a[:, :, :, 0].flatten())

###############################
###############################

if ...:
    print('True')
else:
    print('False')

###############################
###############################
print(...)
```

### f-Strings

```python
x = 10
y = 20

print(f"x = {x}, y = {y}") 
print(f"{x = }, {y = }") 

# math operations
print(f"{x * y = }")

# x = 10, y = 20
# x = 10, y = 20
# x * y = 200
```
Let’s say you have a large number, as large as Apple’s market cap; you can use :, where , is the separator.

Or, if you want f string to print out a percentage value, you can use :.2% telling Python to set 2 decimal places and add a percentage sign to the end of the string.

```python
apple_marketcap = 2.626 * 10e12

print(f"{apple_marketcap = :,}") # comma separator

percentage = 10.394394

print(f"{percentage = :.2%}") # percentage

# apple_marketcap = 26,260,000,000,000.0
# percentage = 1039.44%
```

Date formatting:

```python
import datetime

today = datetime.datetime.utcnow()
print(f"datetime : {today}\n")

print(f"date time: {today:%m/%d/%Y %H:%M:%S}")
print(f"date: {today:%m/%d/%Y}")
print(f"time: {today:%H:%M:%S.%f}") 
print(f"time: {today:%H:%M:%S %p}") 
print(f"time: {today:%H:%M}")
datetime : 2022-09-13 05:44:17.546036

# date time: 09/13/2022 05:44:17
# date: 09/13/2022
# time: 05:44:17.546036
# time: 05:44:17 AM
# time: 05:44
```

```python
# Locale’s appropriate date and time representation
print(f"locale appropriate: {today:%c}")

# weekday
print(f"weekday: {today:%A}")

# day of the year
print(f"day of year: {today:%j}")

# how far are we into the year?
day_of_year = f"{today:%j}"
print(f"progress % year: {int(day_of_year)/365 * 100:.2f}%")

# locale appropriate: Tue Sep 13 05:44:17 2022
# weekday: Tuesday
# day of year: 256
# progress % year: 70.14%
```

Some useful links that helped me to get better at python.

- [PyGame: A Primer on Game Programming in Python | RealPython](https://realpython.com/pygame-a-primer/#game-speed)
- [Python Plotting With Matplotlib (Guide) | RealPython](https://realpython.com/python-matplotlib-guide/)
- [An Intro to Threading in Python | RealPython](https://realpython.com/intro-to-python-threading/)
- [Reading and Writing CSV Files in Python | RealPython](https://realpython.com/python-csv/)
- [Introduction to Git and GitHub for Python Developers | RealPython](https://realpython.com/python-git-github-intro/)
- [Python Command Line Arguments | RealPython](https://realpython.com/python-command-line-arguments/)
- [Python Virtual Environments: A Primer | RealPython](https://realpython.com/python-virtual-environments-a-primer/)
- [medium | 5 Python Features That I Was Unaware Even Existed](https://betterprogramming.pub/python-features-that-i-was-unaware-even-existed-8465a50a6378)























