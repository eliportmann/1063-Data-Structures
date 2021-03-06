Homework 1 - EndSert Method
==========
Due: February 10th by Class time.

## Overview
- Using the [starter.cpp](./starter.cpp) file, add a method called **`EndSert`** that uses a ***tail*** pointer to insert a node at the tail end of the list.
- This means you will need to keep the tail pointer always pointed at the last node. This is not to difficult since you would only need to move the ***tail*** pointer if you use your **`EndSert`** method. Obviously, you need to point ***tail*** to the very first node added to the list as well (see below).
- On the insertion of the value 18, using the **`FrontSert`** or **`EndSert`** methods would result in the same outcome if that value is the first value being added to the list (in regards to the ***head*** and ***tail*** pointers)

### Example

![](https://d3vv6lp55qjaqc.cloudfront.net/items/0U2R2P3R0E0z080R150O/linked_lsit.png?X-CloudApp-Visitor-Id=1094421)

## Deliverables

- Create a file called `tail_insertion.cpp` and place your solution in this file.
- Add your `tail_insertion.cpp` to your `assignments` folder.
- Make sure you place a comment block at the top of your document, as well as a comment block on your added method.

Main Program Comment Block:
```cpp
/**
* @ProgramName: Program-1
* @Author: Your Name 
* @Description: 
*     This program reads in images stored as rgb values in a space delimited file format.
* @Course: 1063 Data Structures
* @Semester: Spring 2017
* @Date: DD MM YYYY
*/
```

Function Comment Block:
```cpp
/**
* @FunctionName: grayScale
* @Description: 
*     Loops through a 2D array and turns every RGB value into its grayscale equivalent.
* @Params:
*    rgb** image - 2D array holding rgb values
*    int width - width of image
*    int height - height of image
* @Returns:
*    void
*/
void grayScale(rgb** image,int width,int height){
    // your code
}
```

- Print out a copy of your code and bring to class. 
