EXP NO:11 C PROGRAM TO DISPLAY STACK ELEMENTS USING AN ARRAY.
NAME: MAHAGAURI P
REG NO: 212224040181
Aim: To write a C program to display stack elements using an array. Algorithm:

Include Necessary Header Files
Declare Global Variables
Define the Display Function
Main Function (or Other Relevant Code)
Initialize the stack and top as needed.
Perform stack operations (push, pop, etc.).
Use the display function to visualize the stack's contents
Program:
```
#include <stdio.h>
#define SIZE 5

int stack[SIZE], top = -1;

void push(int value) {
    if (top == SIZE - 1)
        printf("Stack Overflow\n");
    else
        stack[++top] = value;
}

void display() {
    if (top == -1)
        printf("Stack is empty\n");
    else {
        printf("Stack elements:\n");
        for (int i = top; i >= 0; i--)
            printf("%d\n", stack[i]);
    }
}

int main() {
    push(10);
    push(20);
    push(30);
    display();
    return 0;
}
```
Output:
![1](https://github.com/user-attachments/assets/86e1db17-1fce-4f4f-8f84-55b0e29c0b94)



Result: Thus, the program to display stack elements using an array is verified successfully.

EXP NO:12 PROGRAM TO PUSH THE GIVEN ELEMENT IN TO A STACK USING ARRAY.
Aim: To create a C program to push the given element in to a stack using array. Algorithm:

Declare global variables for the stack size, top index, and the stack itself.
Define the push function to add a floating-point number to the stack.
Initialize the stack size, top index, and the stack itself.
Call the push function as needed.
Program:
```
#include <stdio.h>
#define SIZE 5

int stack[SIZE], top = -1;

void push(int value) {
    if (top == SIZE - 1)
        printf("Stack Overflow\n");
    else {
        stack[++top] = value;
        printf("%d pushed into stack\n", value);
    }
}

int main() {
    push(5);
    push(10);
    push(15);
    return 0;
}
```
Output:

![2](https://github.com/user-attachments/assets/fe56bc84-bef6-40c5-bf35-8fe8e180d94f)


Result:

Thus, the program to push the given element in to a stack using array is verified successfully

EXP NO:13 C PROGRAM TO DISPLAY QUEUE ELEMENTS USING ARRAY.
Aim: To write a C program to display queue elements using array

Algorithm:

Declare global variables for the queue, rear, front, and iteration.
Define the display function to print the elements of the queue.
Initialize the queue, rear, and front as needed.
Call the display function and perform other queue operations as needed.
Program:

```
#include <stdio.h>
#define SIZE 5

int queue[SIZE], front = -1, rear = -1;

void enqueue(int value) {
    if (rear == SIZE - 1)
        printf("Queue Overflow\n");
    else {
        if (front == -1) front = 0;
        queue[++rear] = value;
    }
}

void display() {
    if (front == -1 || front > rear)
        printf("Queue is empty\n");
    else {
        printf("Queue elements:\n");
        for (int i = front; i <= rear; i++)
            printf("%d\n", queue[i]);
    }
}

int main() {
    enqueue(10);
    enqueue(20);
    enqueue(30);
    display();
    return 0;
}
```
Output:

![3](https://github.com/user-attachments/assets/03a536c5-73da-4f45-9dd3-0a75a8f22e85)


Result:

Thus, the program to display queue elements using array is verified successfully.

EXP NO:14 C PROGRAM TO INSERT ELEMENTS IN QUEUE USING ARRAY.
Aim: To write a C program to insert elements in queue using array.

Algorithm:

Declare global variables for the size, rear, front, and the queue itself.
Define the enqueue function to add a float to the queue.
Initialize the rear, front, and size of the queue as needed.
Call the enqueue function as needed.
Program:
```
#include <stdio.h>
#define SIZE 5

int queue[SIZE], front = -1, rear = -1;

void enqueue(int value) {
    if (rear == SIZE - 1)
        printf("Queue Overflow\n");
    else {
        if (front == -1) front = 0;
        queue[++rear] = value;
        printf("%d inserted into queue\n", value);
    }
}

int main() {
    enqueue(5);
    enqueue(10);
    enqueue(15);
    return 0;
}
```
Output:

![4](https://github.com/user-attachments/assets/caf07576-5494-40ca-b5b4-cfcd82a2774f)


Result:

Thus, the program to insert elements in queue using array is verified successfully.

EXP NO:15 C FUNCTION TO DELETE ELEMENTS IN QUEUE USING ARRAY
Aim:

To create a function in C that deletes an element from a queue implemented using an array.

Algorithm:

Check if the Queue is Empty o If the front pointer is -1, it means the queue is empty, and there are no elements to delete. Print a message indicating that the queue is empty.
Delete the Front Element o If the queue is not empty, the element at the front index is deleted. o Increment the front pointer by 1 to remove the element and point to the next element in the queue.
Check if the Queue Becomes Empty After Deletion: o After deletion, check if the front pointer has passed the rear pointer (front > rear). If this is true, reset both front and rear to -1, indicating that the queue is now empty.
End the Function.
Program:
```
#include <stdio.h>
#define SIZE 5

int queue[SIZE], front = -1, rear = -1;

void enqueue(int value) {
    if (rear == SIZE - 1)
        printf("Queue Overflow\n");
    else {
        if (front == -1) front = 0;
        queue[++rear] = value;
    }
}

void dequeue() {
    if (front == -1 || front > rear)
        printf("Queue Underflow\n");
    else
        printf("%d deleted from queue\n", queue[front++]);
}

int main() {
    enqueue(10);
    enqueue(20);
    enqueue(30);
    dequeue();
    dequeue();
    return 0;
}
```

Output:

![5](https://github.com/user-attachments/assets/d2a23028-93d3-48f5-8d65-0f42403dde8c)


Result:

Thus, the function that deletes an element from a queue implemented using an array is verified successfully.
