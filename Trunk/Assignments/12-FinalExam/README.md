# Study Guide
Final Exam: Monday May 8th, 3:30 p.m. - 5:30 p.m.

I uploaded a [final exam](https://github.com/rugbyprof/1063-Data-Structures/blob/master/Assignments/12-FinalExam/CMPS_1053_Final_Exam.fall.12.pdf) from 2012, so you can see that I have actually scaled it back! So be happy :) 

## Pointers

| Memory Snapshot |
|:-------------:|
| ![](https://d3vv6lp55qjaqc.cloudfront.net/items/1s0J3A0J2T3i1l0p2g2b/pointer_memory.png?X-CloudApp-Visitor-Id=1094421) |

| #|Command           | Result |
|--|:-----------------:|:------:|
|1|  `cout<<&D`       |    |
|2|  `cout<<&E`       |  |
|3|  `cout<<*D`       |    |
|4|  `cout<<*F`       |    |
|5|  `cout<<F`        |    |
|6|  `cout<<A`        |        |
|7|  `cout<<*E`       |     |
|8| `cout<<&G`        |      |
|9| `C = &A; cout<<*C`|        |
|10|  `*F=*D; cout<<*F`|        |

<sub>Solution: https://github.com/rugbyprof/1063-Data-Structures/edit/master/Assignments/06-Test-1/test-1-solution.md</sub>

## Arrays
- Write functions to do the following to a an array:
    - Sum integer values 
        - Receives array, its size, and returns the sum of the values.
    - Avg integer values
        - Receives array, its size, and returns the sum of the values.
    - Max integer
        - Receives array, its size, and returns the maximum value in the array.
    - Count occurences of a specified string in an array
        - Receives an array of words, a key to search for, and returns the number of times that key occurs in the array.


## Lists

- What is the worst case search time for a singly linked list? Discuss what advantages / disadvantages a doubly linked list would have for: (1) Searching (2) Inserting (3) Deleting

-----

- Write a c++ function the will return the largest and smallest values from any given linked list.
 - Write a function to merge two linked lists of integers that are sorted into ascending order. The result should be a third linked list that is the sorted combination of the original lists. Do not destroy the original lists. Do not assume you have a class with methods to complete this problem.
 
 ![](https://d3vv6lp55qjaqc.cloudfront.net/items/2k1B1k2J0J0L221g2I2a/Image%202017-05-03%20at%202.26.48%20PM.png?X-CloudApp-Visitor-Id=1094421)
 
 ```cpp
Node * List1; //points to List1 above
Node * List2; //points to List2 above
Node * List3; //currently points to NULL;
List3 = MergeLists(List1,List2); //function call to merge the lists.

//Your function will receive two Node*’s and return a 3rd Node* that points to your new merged list.

Node* MergeLists(Node* L1, Node* L2){


```
-----

- Write a `Count()` function that counts the number of times a given int occurs in a list.

```cpp
void main() {
    List myList;
    myList.BuildOneTwoThree(); // build {1, 2, 3}
    int count = MyList.Count(2); // returns 1 since there's 1 '2' in the list
}
/*
Given a list and an int, return the number of times that int occurs
in the list.
*/
int List::Count(int searchFor) {
// Your code



```
-----

- Write a `Remove()` function that removes the front node from a linked list. Pop takes a non-empty list, deletes the head node, and returns the head node's data. Here is how it could be used:

```cpp
void main() {
    List MyList;
    MyList.BuildOneTwoThree(); // build {1, 2, 3}
    int a = MyList.Remove (); // deletes "1" node and returns 1
    int b = MyList.Remove (); // deletes "2" node and returns 2
    int c = MyList.Remove (); // deletes "3" node and returns 3
    int len = MyList.Length(); // the list is now empty, so len == 0
}
/*
Takes a non-empty list and removes (deletes) the front node, and returns the data which was in that node.
*/
int List::Remove() {
// your code...


```

## Searching 

Use a standard binary search method to find the value 10  within the following array. Do anything necessary to the array to assist in your binary search. At each step, be sure to label the First, Middle, and Last (you can use F,M and L) locations. 

![](https://d3vv6lp55qjaqc.cloudfront.net/items/1M0N0K1h3N0O2T291I3Z/Image%202017-05-03%20at%209.01.01%20PM.png?X-CloudApp-Visitor-Id=1094421)

## Using Stacks And Queues
- Below you see a stack ***`S`*** in its initial state. (For this question: Stack uses ***`Push`*** and ***`Pop`*** )
- A queue ***`Q`*** , in its initial state. (For this question: Queue uses ***`Add`*** and ***`Remove`*** )
- And a list ***`L`*** that’s in its FINAL state. (List uses ***`Add`*** )

![](https://d3vv6lp55qjaqc.cloudfront.net/items/091O2N250w1c2h0S0e1W/Image%202017-05-03%20at%208.49.23%20PM.png?X-CloudApp-Visitor-Id=1094421)

- You need to write a series of `push`, `pops`, `adds`, and `removes` to get the values from ***`S`*** and ***`Q`*** into ***`L`*** in the order displayed. 
- ***`L.Add`*** adds the values to the rear of the list.

## ~~Array Based Stacks and Queues~~
(concentrate on list implementations)
- ~~Write a complete class implementation of an array based stack~~
- ~~Write a complete class implementation of an array based queue~~
- ~~<sub>https://github.com/rugbyprof/1063-Data-Structures/blob/master/Lectures/Day04.cpp</sub>~~

## List Based Stacks and Queues

- Write a complete class implementation of a list based stack
- Write a complete class implementation of a list based queue
- <sub>https://github.com/rugbyprof/1063-Data-Structures/blob/master/Lectures/Day19.cpp</sub>

#### Array vs List
- What are benefits of using an array based implementation?
- What are benefits of using a list based implementation?
- Explain why we need to implement a queue using the "circular" technique when using an array, but not when using a list.

