#  Linked Lists
## What is a Linked List?
#### A Linked List is a sequence of Nodes that are connected/linked to each other. The most defining feature of a Linked List is that each Node references the next Node in the link.
#### linear data structures, which means that there is a sequence and an order to how they are constructed and traversed.
![](https://miro.medium.com/max/700/1*Xokk6XOjWyIGCBujkJsCzQ.jpeg)
#### Memory management
##### when a linked list is born, One byte could live somewhere, while the next byte could be stored in another place in memory altogether! Linked lists don’t need to take up a single block of memory; instead, the memory that they use can be scattered throughout.
![](https://miro.medium.com/max/700/1*G43FVT5xJ1n1QDKVNZUxXQ.jpeg)
#### linked lists are dynamic data structures ;so it  can shrink and grow in memory. It doesn’t need a set amount of memory to be allocated in order to exist, and its size and shape can change, and the amount of memory it needs can change as well.
#### Parts of a linked list:
#####  A linked list is made up of a series of nodes, which are the elements of the list.
+ head.:The starting point of the list is a reference to the first node.
###### Nearly all linked lists must have a head, because this is effectively the only entry point to the list and all of its elements, and without it, you wouldn’t know where to start! The end of the list isn’t a node, but rather a node that points to null, or an empty value.
![](https://miro.medium.com/max/700/1*K0_eV07tJtKQSVGKfP18bw.jpeg)
### A node only knows about what data it contains, and who its neighbor is.
##### A single node is also pretty simple. It has just two parts: data, or the information that the node contains, and a reference to the next node.
#### Lists for all shapes and sizes
+ Singly linked lists :There is a single track that we can traverse the list in; we start at the head node, and traverse from the root until the last node, which will end at an empty null value.
+ doubly linked list:as a node can reference its subsequent neighbor node, it can also have a reference pointer to its preceding node, too! because there are two references contained within each node: a reference to the next node, as well as the previous node.
![](https://miro.medium.com/max/700/1*AeMDLFUjR0w0J4n8CP4H6g.jpeg)
+ circular linked list : This organization structure makes it really easy to add something to the end of the list, because you can begin traversing it at the tail node, as the first element and last element point to one another.
### what even is Big O?
#### Big O Notation is a way of evaluating the performance of an algorithm.
#### There are two major points to consider when thinking about how an algorithm performs: how much time it requires at runtime given how much time and memory it needs.
#### As far as linked lists go, however, the two types of Big O equations to remember are O(1) and O(n).
##### An O(1) function takes constant time, which is to say that it doesn’t matter how many elements we have, or how huge our input is: it’ll always take the same amount of time and memory to run our algorithm. 
##### An O(n) function is linear, which means that as our input grows (from ten numbers, to ten thousand, to ten million), the space and time that we need to run that algorithm grows linearly.
### Growing a linked list
#### So, all we need to do in order to add something to our linked list is figure out which pointer needs to point to where.
+ First, we find the head node of the linked list.
+ Next, we’ll make our new node, and set its pointer to the current first node of the list.
+ Lastly, we rearrange our head node’s pointer to point at our new node.
![](https://miro.medium.com/max/700/1*Jy5tjwrMdtpGl2ceq4f94A.jpeg)
#### Inserting an element at the beginning of a linked list is particularly nice and efficient because it takes the same amount of time, no matter how long our list is, which is to say it has a space time complexity that is constant, or O(1).
#### But inserting an element at the end of a linked list is a different story. The interesting thing here is that the steps you take to actually do the inserting are the exact same:
+ find the node we want to change the pointer of
+ Create the new node we want to insert and set its pointer
+ Direct the preceding node’s pointer to our new node

### To list or not to list?
#### a linked list is usually efficient when it comes to adding and removing most elements, but can be very slow to search and find a single element.





[Github view](https://github.com/sbkhaloof/growthmindsit)



