# Stacks and Queues
## A stack is a linear data structure in which elements can be inserted and deleted only from one side of the list, called the top. A stack follows the LIFO (Last In First Out) principle, i.e., the element inserted at the last is the first element to come out. The insertion of an element into stack is called push operation, and deletion of an element from the stack is called pop operation. In stack we always keep track of the last element present in the list with a pointer called top.

### The diagrammatic representation of stack is given below:
![](https://res.cloudinary.com/practicaldev/image/fetch/s--s1Qbl8Gf--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/mwcwre09s12vqa3gvl7a.png)

## A queue is a linear data structure in which elements can be inserted only from one side of the list called rear, and the elements can be deleted only from the other side called the front. The queue data structure follows the FIFO (First In First Out) principle, i.e. the element inserted at first in the list, is the first element to be removed from the list. The insertion of an element in a queue is called an enqueue operation and the deletion of an element is called a dequeue operation. In queue we always maintain two pointers, one pointing to the element which was inserted at the first and still present in the list with the front pointer and the second pointer pointing to the element inserted at the last with the rear pointer.

![](https://miro.medium.com/max/1838/0*hubLbRXhlN4IBnGN)

## Difference between Stack and Queue Data Structures



![](https://res.cloudinary.com/practicaldev/image/fetch/s--XWnztdhd--/c_imagga_scale,f_auto,fl_progressive,h_900,q_auto,w_1600/https://cl.ly/d84e17fec485/Image%25202018-09-13%2520at%252012.22.09%2520PM.png)





|                                                           Stacks                                           | Queues                                 | 
| :--------------------------------------------------------------------------------------------------------- | :------------------------------------: | 
|Stacks are based on the LIFO principle,                                                                     | Queues are based on the FIFO principle  | 
|Insertion and deletion in stacks takes place only from one end of the list called the top.	                 | Insertion and deletion in queues takes place from the opposite ends of the list. The insertion takes place at the rear of the list and the deletion takes place from the front of the list.| 
|Insert operation is called push operation.                                                                  | Insert operation is called enqueue operation   | 
|Delete operation is called pop operation.                                                                   | Delete operation is called dequeue operation. | 
|one pointer to access the list, called the top, which always points to the last element present in the list.| In queues we maintain two pointers to access the list.frontand rear   | 
|Stack is used in solving problems works on recursion.                                                       | Queue is used in solving problems having sequential processing. |





















[Github view](https://github.com/sbkhaloof/growthmindsit)