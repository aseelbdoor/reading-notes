# Class 09

- What is the basic syntax of Python list comprehension, and how does it differ from using a for loop to create a list? Provide an example of a list comprehension that squares the elements in a given list of integers.
```python
List comprehension is a concise way to create a new list by iterating over an existing iterable (e.g., list, tuple, string) and applying an expression or condition to each element. It provides a more compact and readable alternative to using a for loop to create a list.
The basic syntax of a list comprehension in Python is as follows:
new_list = [expression for element in iterable if condition]
Using list comprehension, you can achieve the same result as a for loop in a more concise and expressive manner.

Here is an example that demonstrates how to square each element in a given list of integers using list comprehension:

numbers = [1, 2, 3, 4, 5]
squared_numbers = [num**2 for num in numbers]
print(squared_numbers)

The output of this code will be:
[1, 4, 9, 16, 25]
```

- What is a decorator in Python?
```python
In Python, a decorator is a design pattern that allows you to modify the behavior of a function or a class without directly changing its source code. It provides a way to add additional functionality or modify the existing functionality of a function or a class dynamically.

A decorator is itself a callable object that takes a function or a class as input and returns a modified version of that function or class. It is denoted using the @ symbol followed by the name of the decorator function or class, placed above the function or class it is decorating.

Decorators are commonly used for tasks such as logging, timing, authentication, and more. They provide a clean and modular way to extend or modify the behavior of functions or classes without altering their core implementation.
```

- Explain the concept of decorators in Python. How do they work, and what are some common use cases for them? Provide an example of a simple decorator function from the reading.
```python
In Python, decorators are a language feature that allows you to modify the behavior of functions or classes by wrapping them with additional functionality. Decorators provide a way to extend or modify the behavior of existing code without directly modifying its source code. They are based on the concept of higher-order functions, where a function takes another function as input and returns a modified version of it.

Decorators in Python work by applying the @decorator_name syntax to a function or class declaration. This syntax tells Python to pass the function or class to the decorator, which then modifies it and returns the modified version. The modified function or class is then used in place of the original one.

Common use cases for decorators include:
1-Logging: Decorators can be used to add logging statements to functions or classes, allowing you to track their execution and debug potential issues.
2-Timing and profiling: Decorators can be used to measure the execution time of functions, helping you identify performance bottlenecks.
3-Caching: Decorators can be used to cache the results of expensive function calls, improving performance by avoiding redundant computations.

def log_execution(func):
    def wrapper(*args, **kwargs):
        print(f"Calling function {func.__name__}")
        result = func(*args, **kwargs)
        print(f"Function {func.__name__} executed")
        return result
    return wrapper

@log_execution
def add_numbers(a, b):
    return a + b
```