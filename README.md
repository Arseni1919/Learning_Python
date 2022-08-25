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

Some useful links that helped me to get better at python.

- [PyGame: A Primer on Game Programming in Python | RealPython](https://realpython.com/pygame-a-primer/#game-speed)
- [Python Plotting With Matplotlib (Guide) | RealPython](https://realpython.com/python-matplotlib-guide/)
- [An Intro to Threading in Python | RealPython](https://realpython.com/intro-to-python-threading/)
- [Reading and Writing CSV Files in Python | RealPython](https://realpython.com/python-csv/)
- [Introduction to Git and GitHub for Python Developers | RealPython](https://realpython.com/python-git-github-intro/)
- [Python Command Line Arguments | RealPython](https://realpython.com/python-command-line-arguments/)
- [Python Virtual Environments: A Primer | RealPython](https://realpython.com/python-virtual-environments-a-primer/)























