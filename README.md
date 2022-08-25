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

Some useful links that helped me to get better at python.

- [PyGame: A Primer on Game Programming in Python | RealPython](https://realpython.com/pygame-a-primer/#game-speed)
- [Python Plotting With Matplotlib (Guide) | RealPython](https://realpython.com/python-matplotlib-guide/)
- [An Intro to Threading in Python | RealPython](https://realpython.com/intro-to-python-threading/)
- [Reading and Writing CSV Files in Python | RealPython](https://realpython.com/python-csv/)
- [Introduction to Git and GitHub for Python Developers | RealPython](https://realpython.com/python-git-github-intro/)
- [Python Command Line Arguments | RealPython](https://realpython.com/python-command-line-arguments/)
- [Python Virtual Environments: A Primer | RealPython](https://realpython.com/python-virtual-environments-a-primer/)























