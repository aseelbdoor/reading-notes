# Data Structures and Algorithms
1- What is 1 of the more important things you should consider when deciding which data structure is best suited to solve a particular problem?
```
It is important to state that no single data structure serves as an optimal solution for all problems. With that in mind, to pick the best data structure to solve a particular problem, we have to take into account what are the operations we are going to perform and how often they are going to be executed. Then, we need to choose the data structure that delivers the best performance trade-off over the tasks we have to accomplish.
For example, my case is: searching on Google Maps for the best way of getting to a local restaurant from my home I think this concept will help me in my structure (The Shortest Path Algorithm).
```


2- How can we ensure that we’ll avoid an infinite recursive call stack?
```
The recursive function should contain two parts (Base Case, Recursive Case) so I can tell the program when I need to stop recursing. The Base Case is when the function does not call itself, but the Recursive Case is when the function calls itself.
```