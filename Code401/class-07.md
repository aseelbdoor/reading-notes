# Class 07
1- Explain the concept of variable scope in Python and describe the difference between local and global scope. Provide an example illustrating the usage of both.
```python
In Python, the term "variable scope" refers to the area of a program where a variable can be accessed and used. The scope of a variable is determined by where it is defined in the code.

In general, there are two types of variable scope in Python: local scope and global scope.

Local scope refers to variables that are defined inside a function. These variables can only be accessed and used within the function in which they are defined. Once the function returns, the local variables are destroyed and their values cannot be accessed from outside the function. Global scope, on the other hand, refers to variables that are defined outside of any function, and can be accessed and used from anywhere in the program. Global variables can be defined by using the global keyword inside a function.
example:

y = 5
x = 5
def my_func():
    global y
    y = y + 10
    x = 2
    print("Inside the function, x is", x)
    print("Inside the function, y is", y)

my_func()
print("Outside the function, y is", y)
print("Outside the function, x is", x)

Inside the function, x is 2
Inside the function, y is 15
Outside the function, x is 5
Outside the function, y is 15
```

2- How do the global and nonlocal keywords work in Python, and in what situations might you use them?
```python
In Python, the global and nonlocal keywords are used to define the scope of variables in functions.

The global keyword is used to indicate that a variable is defined in the global scope, rather than the local scope of a function. When a variable is defined as global, it can be accessed and modified from any part of the program, including from within functions.

The nonlocal keyword is used to indicate that a variable is defined in an outer scope of a function, but not in the global scope. This is useful when you have nested functions, and want to access or modify a variable in an outer function from an inner function.

```

3- In your own words, describe the purpose and importance of Big O notation in the context of algorithm analysis.
```python
Big O notation is an important tool for algorithm analysis that allows us to measure and compare the efficiency of different algorithms. By using Big O notation to analyze and optimize our code, we can write more efficient and scalable programs that are better able to handle large data sets and time-critical applications.
```

4- Based on the Rolling Dice Example, explain how you would simulate a dice roll using Python. Describe how you would use code to calculate the probability of rolling a specific number (e.g., the probability of rolling a 6) over a large number of trials.
```python
To simulate a dice roll using Python, we can use the random module which provides a randint() function to generate a random integer within a specified range.

Here is an example of a Python function to simulate a single dice roll:

import random
def roll_dice():
    return random.randint(1, 6)

In this example, we import the random module and define a function roll_dice() that uses the randint() function to generate a random integer between 1 and 6, simulating a single dice roll.

to calculate number it is very much to explain after long day
```