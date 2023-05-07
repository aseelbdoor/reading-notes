# Class 04

1- What are the key differences between classes and objects in Python, and how are they used to create and manage instances of a class?
```
In Python, a class is a blueprint for creating objects, while an object is an instance of a class.
Classes are used to define the attributes and methods that objects will have, while objects are instances of a class with specific values for those attributes. You can create multiple objects of the same class by calling the class constructor multiple times with different values for the attributes.
```

2- Explain the concept of recursion and provide an example of how it can be used to solve a problem in Python. What are some best practices to follow when implementing a recursive function?
```
Recursion is a programming technique where a function calls itself to solve a problem. It is a powerful technique that is used in many algorithms and data structures.
The general idea behind recursion is to break a problem down into smaller subproblems and solve each subproblem recursively. The recursive function calls itself with a smaller subset of the original problem, until the problem is small enough to be solved without recursion.
Example:
def factorial(n):
    if n == 1:
        return 1
    else:
        return n * factorial(n-1)
some best practices that you should follow to avoid potential issues:
- Ensure that the recursive function has a base case that terminates the recursion. Without a base case, the function will call itself indefinitely and cause a stack overflow error.
- Make sure that each recursive call is on a smaller subset of the problem. - This will ensure that the function converges towards the base case.
- Use proper naming conventions to make the code more readable. For example, in the factorial function above, we named the function 'factorial()' to clearly indicate its purpose.
- Use comments to document the function and its arguments, as well as any assumptions or constraints on the input values.
```

3- What is the purpose of pytest fixtures and code coverage in testing Python code? Explain how they can be used together to improve the quality and maintainability of a project.
```
Pytest fixtures are functions that provide a fixed baseline set of data, test doubles, or resources for use in test functions. They are a powerful feature of the Pytest framework that allow developers to write more effective and efficient tests by providing a way to manage and share test setup and teardown code.

Code coverage, on the other hand, is a measure of how much of a project's source code is executed during testing. It provides developers with valuable insights into which parts of their codebase are being tested and which parts need more attention.

Together, Pytest fixtures and code coverage can be used to improve the quality and maintainability of a Python project in several ways:
- Increased code coverage: By using Pytest fixtures, developers can write more efficient and comprehensive tests that cover a larger percentage of their codebase. Code coverage reports can then be used to identify parts of the code that are not being tested and prioritize testing efforts accordingly.
- Improved test stability: Pytest fixtures ensure that test data and resources are consistent across multiple test functions, which can help improve test stability and reduce the likelihood of false positives or negatives.
- Simplified test setup and teardown: Pytest fixtures provide a way to manage complex test setup and teardown code, making it easier to write and maintain tests. This can save developers time and reduce the likelihood of errors in test code.
- Better test isolation: Pytest fixtures can be used to isolate tests from each other by providing separate instances of test data or resources. This helps ensure that tests are not dependent on each other and can be run independently, which can improve test reliability.
```
