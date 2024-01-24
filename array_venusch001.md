# Array Documentation (C++)

## ⭐ introduction
 1. arrays are the simplest data structure that one encounters when one starts a course in any language and study dsa.
 2. ok, let me give you a brief of the roadmap of dsa so that you get familiar with the sequencing of the dsa course that exactly where arrays lie. While studying any language like c++, c , python , java etc one gets to study the following:
- basic language
- arrays and strings
- linked list
- trees
- graphs
- more advanced algorithms

## ⭐ everything about arrays
1. arrays can be visualised as a continuos box of containers. these containers can have elements inside them.
2. these containers are situated side by side i.e we can say that arrays have contiguous memory location.
3. the elements present in the array are of the same type and that will depend on how we have declared our array.
4. for example : int arr[10]  

    This means that we have declared an array which has name="arr"
    and size ="10" and the elements stored in the array will be integers only

## ⭐ different varieties of arrays
#### 1. 1D array
this can be visualised as a single row of containers placed side by side
#### 2. 2D array
this can be visualised as if containers are present along the row and column 
#### 3. 3D array
this can be visualised as if containers are present along the length,breadth and height of the array.

## ⭐ operations in our array
 1. declaring the array  
 2. inserting elements in the array(at first , at last , at random position)  
 3. deleting the elements in the array(at first , at last and at the random position)  
 4. sorting the elements in the array  
 5. performing linear and binary search in the array  
 6. finding palindromes , duplicate number , maximum element , minimum element   
 7. finding prime , composite , even , armstrong etc.  


 These are the basic programs for making array's fundamentals to be crystal clear for you.

## ⭐ Upgradation of array
**Problem with arrays**
1.  Arrays have a fixed size, making them less flexible for handling dynamic or varying data.

2.  Arrays require manual memory management, increasing the risk of errors like buffer overflows or memory leaks. So we cannot delete element from the array without writing the extra code for managing the size of the array.

3.  Arrays lack inherent size information, leading to potential bugs in tracking and managing array size.

**Is there any way forward ?**
vector is a dynamic array implementation in C++. It is part of the Standard Template Library (STL) and provides a flexible and efficient alternative to static arrays

1. **Dynamic Resizing:** Vectors automatically resize themselves, eliminating the need for manual memory management. Arrays have a fixed size that needs to be declared beforehand.

2. **Ease of Use:** Vectors provide convenient member functions like push_back() and pop_back() for adding and removing elements, making them more user-friendly.

## ⭐Parting notes 
Arrays are fundamental data structures in programming. 
We have to understand them well so as to move ahead in the roadmap of dsa i provided at the begining of this documentation.




