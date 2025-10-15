# DataStructures-TimeComplexity

## Overview
This project implements several fundamental data structures and sorting algorithms in C++ to explore their efficiency, time complexity, and underlying logic. The implemented components include:

- **Bubble Sort**
- **Heap Sort**
- **Doubly Linked List**
- **Quadratic Hashing**

Each structure and algorithm demonstrates a different approach to data organization, searching, and sorting — providing insight into their trade-offs in performance and complexity.

## Data Structures: Doubly Linked List & Hashing Using Quadratic Probing

In order to see the Big O time complexity of these two data structures, their insertion and search times were recorded in nanosecond using the following librarys:
```cpp
#include <chrono>
#include <time.h>
using namespace std::chrono;
```
Findings can be found in the Csci2270_FinalProject_PartA_ChandlerPhillips.pdf File

To Run with data by yourself, download the files for whichever data structure you want to test and run the following in the terminal of project directory:

Doubly Linked List:
```terminal
g++ -std=c++11 dlldriver.cpp dll.cpp -o dlldriver && ./dlldriver dataSetA.csv
```
==Results==

Insertion of 100 random elements: O(1)

Search of 100 random elements: O(n)

Quadratic Hashing: 
```
g++ -std=c++11 hashquaddriver.cpp hashquad.cpp -o hashquad && ./hashquad dataSetA.csv
```
==Results==

Insertion of 100 random elements: O(1)

Search of 100 random elements: O(1)

## Data Structures: Bubble & Heap Sort

Using the same libraries previously metioned, used a similar method to get the time (in nanoseconds) of how long these sorting algorithms took to sort 10,000 elements.

Findings can be found in the Csci2270_FinalProject_PartB_ChandlerPhillips.pdf File

To Run with data by yourself, download the files for whichever sorting algorithim you want to test and run the following in the terminal of project directory:

Bubble Sort:
```terminal
g++ -std=c++11 bubblesortdriver.cpp bubblesort.cpp -o bubblesort && ./bubblesort dataSetA.csv
```
==Results==

O(n<sup>2</sup>)

Heap Sort: 
```
g++ -std=c++11 heapsortdriver.cpp heapsort.cpp -o heapsort && ./heapsort dataSetA.csv
```
==Results==

O(n log n)




