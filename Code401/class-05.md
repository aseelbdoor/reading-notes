# Big O: Analysis of Algorithm Efficiency

it describe the worst case of the efficiency of an algorithm and this efficiency evaluated based on **Running time** or the time complexity and **Memory space** or the space complexity 

To analyze the time and space limiting factors, we should consider 4 Key Areas for analysis:

+ Input Size

refers to the size of the parameter values that are read by the algorithm.

+ Units of Measurement

for Running Time :

    - The time in milliseconds from the start of a function execution until it ends
    - The number of operations that are executed.
    - The number of “Basic Operations” that are executed


for Memory space :

    - The amount of space needed to hold the code for the algorithm
    - The amount of space needed to hold the input data
    - The amount of space needed for the output data
    - The amount of space needed to hold working space during the calculation

## Linked Lists

a linear collection of data elements whose order is not given by their physical placement in memory. Instead, each element points to the next.

## Linked list types 
In Python, there are several types of linked lists that can be implemented:

- Singly Linked List: A singly linked list is the simplest type of linked list, in which each node contains a reference to the next node in the list. The first node is called the head of the list, and the last node has a reference to None.

- Doubly Linked List: A doubly linked list is similar to a singly linked list, but each node has a reference to both the next and the previous nodes. This allows for more efficient traversal in both directions, but also requires more memory to store the additional references.

- Circular Linked List: A circular linked list is a variation of a linked list in which the last node in the list has a reference to the first node, creating a circular structure. This can be useful in certain applications, such as implementing a round-robin scheduler.

- Skip List: A skip list is a probabilistic data structure that can be used to implement a sorted list in which each node contains multiple references to other nodes at different levels of the list. This allows for efficient searching and insertion of elements in the list.

## Parts of a linked list
A linked list is made up of a series of nodes, each of which contains two parts:

- Data part: This part of the node holds the value or data that the node represents, such as an integer, string, or other data type.
- Pointer part: This part of the node holds a reference to the next node in the list. In a doubly linked list, the node also has a pointer to the previous node in the list.

### Linear data structures VS Non-linear data structures

**linear data structures** : means that there is a sequence and an order to how they are constructed and traversed

**non-linear data structures** : means that we could traverse the data structure non-sequentially.


## Big O for linked list 

* Inserting an element at the beginning of a linked list is particularly nice and efficient because it takes the same amount of time, no matter how long our list is, which is to say it has a space time complexity that is constant, or O(1). 

* But inserting an element at the end of a linked list we will follow these steps :
    - Find the node we want to change the pointer of (in this case, the last node)
    - Create the new node we want to insert and set its pointer (in this case, to null)
    - Direct the preceding node’s pointer to our new node