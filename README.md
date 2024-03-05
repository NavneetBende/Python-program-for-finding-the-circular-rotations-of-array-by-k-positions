Circular rotation of an array by K position
Here in this program, we will learn about Python program for finding the circular rotations of array by k positions, which means rotating the elements in the array .The operation of the rotation moves the last element of the array to the first position and moves all the remaining elements to the right. Take into consideration the following [0,1,2] indexes to be checked.

Python program for finding the circular rotations of array by k positions
Keypoint
In this section we will learn about basic knowledge which we need to know before coding the above Program. So we must have knowledge of what is an array? 

What is an array?
An array is a data structure, it is collection of similar data elements which is stored at contiguous memory locations in which each data element can be accessed directly by only using its index number.
 
About Python language:-
Python is a popular programming language. Python is a high level language that will make a programmer focus on what to do instead of how to do.
Its design philosophy emphasizes code readability with its use of significant indentation. Its language constructs as well as its object-oriented approach aim to help programmers write clear, logical code for small and large-scale 
 
 
How to declare an array?
To declare an array in C,a programmer specifies the type of the elements and the number of elements required by an array as follows − This is called a single-dimensional array. The arraySize must be an integer constant greater than zero and type can be any valid C data type. For example, to declare a 10-element array called balanceof type double, use this statement − Here balanceis a variable array which is sufficient to hold up to 10 double numbers
Algorithm of Python program for finding the circular rotations of array by k positions
Algorithm
Step 1- Initialize a class

Step 2- Enter number of elements of array

Step 3- Enter number of rotations of array.

Step 4- Enter number of indexes to be displayed.

Step 5- Input array elements

Step 6- run a for loop, i=0; i< elements; , i++.

Step 7- then module your rotations with elements

Step 8- Enter the index of array to be displayed

Step 9- print number of indexes and rotations.

 
Circular Rotations Of Array By K Positions
Code for Python program for finding the circular rotations of array by k positions
def rotateArray(arr, n, d):
    temp = []
    i = 0
    while (i < d):
        temp.append(arr[i])
        i = i + 1
    i = 0
    while (d < n):
        arr[i] = arr[d]
        i = i + 1
        d = d + 1
    arr[:] = arr[: i] + temp
    return arr# Driver function to test above function arr = [1, 2, 3, 4, 5] print(“Array after left rotation is: “, end=’ ‘) print(rotateArray(arr, len(arr), 2))
Output
Array after left rotation is: [3, 4, 5, 1, 2]
