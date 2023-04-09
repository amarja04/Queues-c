# Queues-c

Queue is an abstract data structure, somewhat similar to Stacks. Unlike stacks, a queue is open at both its ends. One end is always used to insert
data (enqueue) and the other is used to remove data (dequeue).

Queue follows First-In-First-Out (FIFO) methodology, i.e., the data item stored first
will be accessed first.

![image](https://user-images.githubusercontent.com/125913981/230798228-3a4eff6a-6477-47bd-8428-2b7ff6c0a4ee.png)

In the above image, since 1 was kept in the queue before 2, it is the first to be removed from the queue as well. It follows the FIFO rule.

In programming terms, putting items in the queue is called enqueue, and removing items from the queue is called dequeue.


Basic Operations of Queue

A queue is an object (an abstract data structure - ADT) that allows the following operations:

Enqueue: Add an element to the end of the queue

Algorithm:

       procedure  enqueue (data)

                if   queue is full
     
                         return OVERFLOW
     
        endif
 
                  rear<-- rea+1
   
                  queue[rear] <-- data
   
           return true
   
    end procedure


Dequeue: Remove an element from the front of the queue

Algorithm:

       procedure  dequeue

                if   queue is empty
     
                         return UNDERFLOW
     
        endif
 
                  data = queue[front]
   
                 front <-- front+1
   
           return true
   
    end procedure
    
    
    
IsEmpty: Check if the queue is empty
 
      begin procedure isempty

         if front is less than MIN OR front is greater than rear
  
               return true 
  
     else
  
          return false

        endif

     end procedure
 
 
IsFull: Check if the queue is full

     begin procedure isfull

           if rear equals to MAXSIZE
  
               return true 
  
     else
     
          return false

       endif

     end procedure
 
 
Peek: Get the value of the front of the queue without removing it.

    begin procedure peek

        return queue [front] 
  
      end procedure
