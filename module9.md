**EXP NO:11 C PROGRAM TO DISPLAY STACK ELEMENTS USING AN ARRAY.**

Aim:

To write a C program to display stack elements using an array.

Algorithm:

1.	Include Necessary Header Files

2.	Declare Global Variables

3.	Define the Display Function

4.	Main Function (or Other Relevant Code)

5.	Initialize the stack and top as needed.

6.	Perform stack operations (push, pop, etc.).

7.	Use the display function to visualize the stack's contents
 
Program:
```
char stack[100];
int top,i;
void display()
{
    for(i=top;i>=0;i--)
    {
        printf("%c ",stack[i]);
    }
    if(top ==-1)
    {
        printf("stack is empty\n");
    }
}
```
Output:

![WhatsApp Image 2025-04-27 at 16 20 23_544d36f9](https://github.com/user-attachments/assets/61bc0cc4-50d3-47c8-89ab-65d79bc86798)



Result:
Thus, the program to display stack elements using an array is verified successfully.
 

**EXP NO:12  PROGRAM TO PUSH THE GIVEN ELEMENT IN TO A STACK USING ARRAY.**

Aim:

To create a C program to push the given element in to a stack using array.

Algorithm:

1.	Declare global variables for the stack size, top index, and the stack itself.

2.	Define the push function to add a floating-point number to the stack.

3.	Initialize the stack size, top index, and the stack itself.

4.	Call the push function as needed.
 
Program:
```
int size=3,top=-1,stack[100];
void push (int data)
{
    stack[++top]=data;
}
```
Output:

![WhatsApp Image 2025-04-27 at 16 21 21_c769d34c](https://github.com/user-attachments/assets/b66ce280-4742-4df6-8a58-a4f1131a9918)


Result:
Thus, the program to push the given element in to a stack using array is verified successfully


 
**EXP NO:13 C PROGRAM TO DISPLAY QUEUE ELEMENTS USING ARRAY.**

Aim:

To write a C program to display queue elements using array

Algorithm:

1.	Declare global variables for the queue, rear, front, and iteration.

2.	Define the display function to print the elements of the queue.

3.	Initialize the queue, rear, and front as needed.

4.	Call the display function and perform other queue operations as needed.

 
Program:
```
float queue[50];
int front,rear;
void display()
{
    if(front==-1 && rear==-1)
    {
        printf("No elements to display\n");
    }
    else
    {
        for(int i=front;i<=rear;i++)
        {
            printf("%.1f\n",queue[i]);
        }
    }
    
}
```
Output:

![WhatsApp Image 2025-04-27 at 16 22 02_be5d7d85](https://github.com/user-attachments/assets/34198460-7d90-43b7-a90a-651a48648e6b)


Result:
Thus, the program to display queue elements using array is verified successfully.


 
**EXP NO:14 C PROGRAM TO INSERT ELEMENTS IN QUEUE USING ARRAY.**

Aim:

To write a C program to insert elements in queue using array.

Algorithm:

1.	Declare global variables for the size, rear, front, and the queue itself.

2.	Define the enqueue function to add a float to the queue.

3.	Initialize the rear, front, and size of the queue as needed.

4.	Call the enqueue function as needed.

Program:
```
int front;
int rear;
char queue[50];
void enqueue(char data)
{
    if(front==-1)
    {
        front=0;
    }
    rear++;
    queue[rear]=data;
}
```
Output:

![WhatsApp Image 2025-04-27 at 16 22 53_ef692cd8](https://github.com/user-attachments/assets/e38868c0-1a9b-4e55-a038-c88f087de1c3)


Result:
Thus, the program to insert elements in queue using array is verified successfully.



 
**EXP NO:15 C FUNCTION TO DELETE ELEMENTS IN QUEUE USING ARRAY**



Aim:

To create a function in C that deletes an element from a queue implemented using an array.

Algorithm:

1.	Check if the Queue is Empty
o	If the front pointer is -1, it means the queue is empty, and there are no elements to delete. Print a message indicating that the queue is empty.

2.	Delete the Front Element

o	If the queue is not empty, the element at the front index is deleted.

o	Increment the front pointer by 1 to remove the element and point to the next element in the queue.

3.	Check if the Queue Becomes Empty After Deletion:

o	After deletion, check if the front pointer has passed the rear pointer (front > rear). If this is true, reset both front and rear to -1, indicating that the 
queue is now empty.

4.	End the Function.



Program:
```
float queue[50];
int front, rear;
void dequeue()
{
    if(front==-1 && rear==-1){
        printf("Queue Underflow.\n");
    }
    else if(front<rear)
    {
        front++;
    }
    else
    {
        front=-1;
        rear=-1;
        printf("No elements to display");
    }
}
```
Output:

![WhatsApp Image 2025-04-27 at 16 23 59_faad158d](https://github.com/user-attachments/assets/64cf7561-1bcd-4ffd-a48b-908566cc15c4)

Result:
Thus, the function that deletes an element from a queue implemented using an array is verified successfully.
