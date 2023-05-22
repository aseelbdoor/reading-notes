# Class 10
What is the purpose of dunder methods in Python? Provide an example of a commonly used dunder method.
```python
Dunder methods (double underscore methods), also known as magic methods or special methods, are predefined methods in Python that provide special functionality to classes. These methods are surrounded by double underscores, hence the name "dunder methods." They allow classes to emulate built-in behaviors or operations, making objects of those classes behave like native Python objects.

One commonly used dunder method is the __init__ method. It is used as a constructor for a class and is executed automatically when an object is created from the class. It allows you to initialize the attributes of the object.
```

In the video “AI Guru makes $238,800 with misleading paid course,” what was the main ethical issue raised concerning the use of developers’ work, and how might this have been avoided?
```python
when it comes to ethical issues concerning the use of developers' work, one of the main concerns is plagiarism or unauthorized use of someone else's code or intellectual property without proper attribution or permission. This can lead to issues related to intellectual property rights, fairness, and trust within the developer community.
To avoid such ethical issues, it is important for developers and content creators to:

- Respect intellectual property rights: Always give credit to the original authors and obtain proper permission when using someone else's work. Follow licensing terms and adhere to open-source guidelines if applicable.

- Clearly define ownership and licensing: Clearly specify the ownership and licensing terms for any code or work created. This helps establish expectations and allows others to understand how they can use or build upon the work.

- Provide proper attribution: When using or referencing others' work, give appropriate credit and acknowledgment. This helps maintain transparency and promotes a collaborative and ethical development community.

- Seek permission when necessary: If intending to use someone else's work extensively or in a commercial context, it's best to seek explicit permission to ensure compliance with ethical and legal standards.
```

Describe the Python statistics module and give an example of a function within the module that can be used to perform a common statistical operation.
```python
The Python statistics module is a built-in module that provides a set of functions for performing various statistical operations. It offers a range of statistical functions to calculate measures of central tendency, dispersion, correlation, and more. The module works with numerical data and operates on sequences like lists, tuples, or other iterable objects.

Here is an example of a function within the statistics module:

import statistics

data = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

# Calculate the mean of the data
mean_value = statistics.mean(data)
print("Mean:", mean_value)

# Calculate the median of the data
median_value = statistics.median(data)
print("Median:", median_value)

# Calculate the standard deviation of the data
std_dev = statistics.stdev(data)
print("Standard Deviation:", std_dev)
```