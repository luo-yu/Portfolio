Author
==========
"Luo, Yu"
Portfolio
=========

Documentation of my course projects, personal project, etc...

Body of portfolio
====

Use Java programing language, basic to object-oriented concepts
----
<li>Please see: https://github.com/luo-yu/SchoolWorks/tree/master/Object-OrientedLanguage</li>

Use Java in data communication (TCP, UDP)
----
<li>Created a simple Tic Tac Toe game. Please see: https://github.com/luo-yu/DataCommunication/tree/master/TicTacToe  </li>
<li>Created a spacewar game, a 2d multi-thread game. Please see: https://github.com/luo-yu/DataCommunication/tree/master/SpaceWar</li>

Use C++ programing language, basic to object-oriented concepts
----
<li>Please see: https://github.com/luo-yu/SchoolWorks/tree/master/Fall2014/cs216</li>

Use PHP with MySQL 
----
<li>Created a simple CMS website. Please see:  https://github.com/luo-yu/CS405G_Project/tree/santa/santa</li>


Use Android SDK
----
<li>Created a simple clipboard Android app. Please see: https://github.com/luo-yu/AndroidProjects/tree/master/Chippet</li>


Create an implementation of a Queue
----
<li> Implementation of a Queue. Please see: https://github.com/luo-yu/SchoolWorks/tree/master/DataAbstractionStructure/03_Queue_Lab</li>

<li> Use a queue as my data structure in the Shuffle project. Please see: https://github.com/luo-yu/SchoolWorks/tree/master/DataAbstractionStructure/Shuffle</li>


Create an implementation of a List
----
<li>Implementation of a List, Please see: https://github.com/luo-yu/SchoolWorks/tree/master/DataAbstractionStructure/04_Linked_List_Lab</li>

Create an implementation of a Binary Search Tree
----
<li>Implementation of a Binary Search Tree, Please see:https://github.com/luo-yu/SchoolWorks/tree/master/DataAbstractionStructure/06_BST_Lab</li>

Create an implementaiton of a Hash Table
----

<li>Implementation of a Hash Table, Please see: https://github.com/luo-yu/SchoolWorks/tree/master/DataAbstractionStructure/05_Hashing_Lab</li>

Create an implementation of a Heap
----
<li>Implementation of a Heap, Please see: https://github.com/luo-yu/SchoolWorks/tree/master/DataAbstractionStructure/07_Heap_Lab </li>


Create an implementation of either Adjanency Lists or Adjacency Matrices
----

<li>Implementation of a Adjacency List, Please see: https://github.com/luo-yu/SchoolWorks/tree/master/DataAbstractionStructure/08_Graph_Lab </li>


Implement graph algorithms
----
<li>Implement graph algorithms, Please see: https://github.com/luo-yu/SchoolWorks/tree/master/DataAbstractionStructure/08_Graph_Lab </li>


Determine space and time requirements of common data structure methods
-----

<li>Please see running time analysis section in my 03_Queue_Lab: https://github.com/luo-yu/SchoolWorks/tree/master/DataAbstractionStructure/03_Queue_Lab</li>

<li>Please see running time analysis section in my 04_Linked_List_Lab: https://github.com/luo-yu/SchoolWorks/tree/master/DataAbstractionStructure/04_Linked_List_Lab</li>

<li>Please see running time analysis section in my 05_Hashing_Lab: https://github.com/luo-yu/SchoolWorks/tree/master/DataAbstractionStructure/05_Hashing_Lab</li>

Describe memory management in C++, and correctly use dynamic variables, including destructors
----
<li>I will explain the dynamic memory management in 04_Linked_List_Lab, please see: https://github.com/luo-yu/SchoolWorks/tree/master/DataAbstractionStructure/04_Linked_List_Lab</li>

<li>In C++, a pointer is a data type that stores the address of another stored value in memory. The Heap and the Stack are two parts in the RAM. The Stack is used to hold the local variables, the return values, and the return addresses from each time I call a function. I cannot use the Stack for things that want to live on. In my lab, all the local variables within every function will be allocated onto the Stack in the RAM. These local variables will be added to the stack at running time in a Last in First out (LIFO) order. </li>

<li>The Heap is the dynamic allocated memory. I can dynamically allocate variables into the heap. In C++, I have to manage the Heap. It is my responsibility that if I allocated a memory in the Heap, I also need to de-allocated when I no longer needed it. In C++, I use the keyword new to allocate memory. In my Lab, I allocated dynamic memory on the heap to a new Node named dummyNode in the constructor using the keyword new. The variable dummyNode is actually a pointer that points to a space in the Heap. When I am done with everything, it is my responsibility to de-allocate this dummyNode. So, in my destructor, I used the keyword delete to de-allocated dummyNode from the Heap. In the add method, I allocated a space for the newly added node named addedNode using the keyword new. This addedNode is a pointer points to a space that exists on the Heap. In the remove method, when I remove an item at position i, I deleted the allocated space on the heap for removed item. I freed all the dynamic memory allocations in the destructor using a while loop, including the dummyNode. My program will not leak memory because every time I remove an item at position i, I will delete the associated memory allocation.
</li>

Create collection classes using templates in C++
----
<li>Please see:https://github.com/luo-yu/SchoolWorks/tree/master/DataAbstractionStructure/04_Linked_List_Lab </li>

<li>In C++, templates are a way to make code more reusable. Function templates are special functions that can operate with generic types. This allows the programmers to create a function template whose functionality can be adapted to more than one type or class without repeating the entire code for each type. To create a template function, we use “template <class type>” on top of the function header. In my lab, the template function is placed within the “LinkedList.ipp” file. The class type T is a generic type; this means that we can reuse these template functions for different types later on. Normally we put declarations in the .h file and the code in a matching .cpp file. Unfortunately, when working with templates, this doesn’t work very well. If we try to compile a “LinkedList.cpp” file with template functions in it, the compiler will not know what a type “T” is, and so the compile will fail. This is because .cpp files are compiled independently.  So when we use template class in C++, we have to include the source code in the “LinkedList.ipp” at the end of the “LinkedList.h” file. </li>


Using time and space analysis, justify the selection of a data structure for a given application
----
<li>Here is my Shuffle project. Please see: https://github.com/luo-yu/SchoolWorks/tree/master/DataAbstractionStructure/Shuffle</li>

In the Shuffle project, I was asked to use a data structure to simulate the shuffling a deck of cards. I chose to use an array based queue to simulate a Hindu shuffle. The Hindu shuffle rearranges the order or the cards in segments. So in order to simulate a Hindu shuffle, there is one important operation is needed. That is, I need to splice a segment (chunk) of cards from the deck and place the segment (chunk) into appropriate position in the deck. 

There are two data structure can be used for this project, an array based queue and a linked list. As I stated, I chose to use an array based queue instead of a linked list. The reason I chose the queue is because that I believed that there was no particular advantages using linked list than using array based queue. 

If I used a linked list, I need to use a splice method. In my 04_LinkedList_Lab, I have a splice method. This splice method will remove several consecutive nodes and insert into the target list at a specified position. However, this splice method takes linear running time, O (n), where n is the index position in the targeted linked list. Most of the operation in this splice method takes constant time; however, this splice method calls a find method. With linked list, a find operation will take linear time because I need to traverse to a particular position in the target list. Since I did a Hindu shuffle, I need to splice a segment of cards in the front of the original linked list, and I need to place this segment at the end of the target list. This means that the find method will have to traverse the whole target list. 

I used an array queue for the Hindu shuffle. I used the array queue from my 03_Queue_Lab. With the array queue, when I do a splice, I remove a segment of cards from the queue, which takes O(n), where n is the number of cards in the segments. I repeatedly doing this until that the queue is empty. So the total cost for the splice operation takes O (m*n), where m is the number of segments, and n is the number of cards in each segments. Even though it takes (m*n), but m will be a constant number, considering that a deck of cards only have 52 cards. For example, if each segment is 20 cards, then m will be just 2.6. So, the splice operation actually takes O (n) time. Therefore, when doing the splice operation for the Hindu shuffle, using linked list has not particular advantages over using an array-based queue. 

<strong><em>Closest Starbucks<em></strong>
Two possible data structures can be used for the Closest Starbucks project (https://github.com/luo-yu/ClosestStarbucks), KD-Trees and Grid (2-d array used as dictionary).  In this project, the data structure must support getNearest() operation.  This method will find and return a nearest location relative to a particular position. 


Using 2-d tree, all the locations are stored as nodes. These nodes are not stored in the internal nodes. The internal nodes do not contain Starbucks locations. They only contain the middle point of x-axis (latitude) and y-axis (longitude).

The choice between 2-d tree and 2-d array depends on the input data set. In this project, the input data set contains Starbucks locations identified by their address, longitude, and latitude. The data set is not sorted. Instead, the data set is randomly distributed. In this case, using 2-d tree is better choice.  Using 2-d tree, the getNearest() will return a pretty accurate location, and it should also be fairly fast.  Getting the nearest location is an O (log N) operation since the input data set contains randomly distributed locations. If using 2-d array for the same input data set, getting the nearest location will be an O (n) operation. 

If the input data set is sorted, then using Grid (2-d array) would be better. Using 2-d array with sorted locations, find a nearest location is an O (1) operation and it will also be very accurate. 

