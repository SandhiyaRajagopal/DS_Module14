# Ex6 Dequeue Elements from Circular Queue
## DATE:25/08/25
## AIM:
To write a C program to delete three elements from the filled circular queue.

## Algorithm
1. Start
2. Check if the queue is empty (front == -1).If empty, print “Queue Underflow” (or return an error value) and exit.
3. Otherwise, store the element at position items[front] into a variable element.
4.  Check if the queue has only one element (front == rear).
     If yes, reset front = -1 and rear = -1 (queue becomes empty).
5. If more than one element is present, move the front pointer forward using circular increment:
      front = (front + 1) % SIZE.
6.Return the value of element.
7. End

## Program:
```
/*
Program to delete three elements from the filled circular queue
Developed by: SANDHIYA R
RegisterNumber: 212223240146 
*/
/*#include <stdio.h>

#define SIZE 5

int items[SIZE];
int front = -1, rear = -1;
*/
int deQueue() 
{
  int element;
  element=items[front];
  if(front==rear)
  {
      front=-1;
      rear=-1;
  }
  else
  {
      front=(front+1)%SIZE;
  }
  return element;
}

```

## Output:

<img width="1145" height="468" alt="image" src="https://github.com/user-attachments/assets/7e6c7cd5-835b-4839-bd7f-453037017359" />


## Result:
Thus, the C program to delete three elements from the filled circular queue is implemented successfully.
