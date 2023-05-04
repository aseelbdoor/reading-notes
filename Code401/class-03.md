1- What is the purpose of the ‘with’ statement when opening a file in Python, and how does it help manage resources while reading and writing files?
```
'with' statement is used to manage resources, such as files, that need to be cleaned up or released after use. It provides a convenient way to ensure that resources are properly released, even if an error occurs during the execution of the code.

When opening a file using the 'with' statement, the file is automatically closed at the end of the with block. 
```

2- Explain the difference between the ‘read()’ and ‘readline()’ methods for file objects in Python. Provide examples of when to use each method.
``` 
The 'read()' method reads the entire contents of the file as a single string, and returns it.

The 'readline()' method reads a single line from the file, and returns it as a string. 
```

3- Briefly describe the concept of exception handling in Python. How can the ‘try’, ‘except’, and ‘finally’ blocks be used to handle exceptions and ensure proper execution of code? Provide a simple example.
```
In Python, exception handling is a mechanism that allows you to gracefully handle errors or exceptions that might occur during the execution of your code. Exceptions are raised when a program encounters an error or a situation that it doesn't know how to handle.

The 'try', 'except', and 'finally' blocks are used to handle exceptions in Python. Here's how they work:
- The 'try' block contains the code that might raise an exception.
- The 'except' block is executed if an exception is raised in the try block. This block contains the code that handles the exception.
- The 'finally' block is executed regardless of whether an exception is raised or not. This block contains the code that should always be executed, even if an exception is raised.
```
# Example of exception handling
```
try:
    num1 = int(input("Enter a number: "))
    num2 = int(input("Enter another number: "))
    print(num1/num2)
except ZeroDivisionError:
    print("Error: Cannot divide by zero!")
finally:
    print("Program finished")
```