# Module-12-Lab-Assignment



EXP NO 26: C PROGRAM TO DISPLAY STACK ELEMENTS USING LINKED LIST.
Aim:
To write a C program to display stack elements using linked list.

Algorithm:
1.	Define a structure Node with two members: data to store the integer value and next to point to the next node in the linked list.
2.	Declare a global variable head representing the starting node of the linked list.
3.	Define a function display to print the elements of the linked list.
4.	Declare a pointer p and initialize it with the head of the linked list.
5.	Use a while loop to traverse the linked list:
6.	Print the data of the current node.
7.	Move to the next node using the next pointer.
 
Program:
```
struct Node   
{  
float data;  
struct Node *next;  
}*head;  
void display()  
{  
    if(head==NULL)
    {
        printf("List is empty");
    }
    else{
        
        struct Node*temp=head;
        while(temp!=NULL){
            printf("%.2f\n",temp->data);
            temp=temp->next;
        }
    }
}
```
Output:

![image](https://github.com/user-attachments/assets/d864f9fa-e752-42b3-9c9c-d22aab3af4ad)

Result:
Thus, the program to display stack elements using linked list is verified successfully. 



EXP.NO 27: C PROGRAM TO POP AN ELEMENT FROM THE GIVEN STACK USING 
LINKED LIST.
Aim:
To write a C program to pop an element from the given stack using liked list.

Algorithm:
1.	Check for Empty Stack
2.	If head is equal to NULL, Print "Stack is empty."
3.	Else Proceed to the next step.
4.	Set head to point to the next node in the stack.
 
Program:
```
struct Node   
{  
float data;  
struct Node *next;  
}*head;  
void pop()  
{
    
    if(head==NULL)
    {
        printf("stack is empty");
    }
    else{
        struct Node* temp = head;
        head = head->next; 
        free(temp);
        
    }
}
```
Output:

![image](https://github.com/user-attachments/assets/1da994d1-7c1a-497f-8889-1206dc779f5a)

Result:
Thus, the program to pop an element from the given stack using liked list is verified successfully.

 
EXP NO:28 C PROGRAM TO DISPLAY QUEUE ELEMENTS USING LINKED LIST.
Aim:
To write a C program to display queue elements using linked list.
Algorithm:
1.	Check if Queue is Empty
2.	Display Queue Elements
3.	Print the data of the current node pointed to by front
4.	Update front to point to the next node.
5.	End the display function.
 
Program:
```
struct Node   
{  
float data;  
struct Node *next;  
}*head;  
void display()  
{  
    if(head==NULL)
    {
        printf("List is empty");
    }
    else{
        
        struct Node*temp=head;
        while(temp!=NULL){
            printf("%.3f\n",temp->data);
            temp=temp->next;
        }
    }
}

Output:

```
![image](https://github.com/user-attachments/assets/f1b44a05-b74f-4989-9523-d45a5975c57f)

Result:
Thus, the program to display queue elements using linked list is verified successfully.


 
EXP NO:29 C PROGRAM TO INSERT ELEMENTS IN QUEUE USING LINKED LIST

Aim:
To write a C program to insert elements in queue using linked list

Algorithm:
1.	Allocate Memory for New Node
2.	Set Data and Next Pointer
3.	Check if Queue is Empty
4.	Set both front and rear to point to the new node p.
5.	Set the next pointer of the current rear to point to the new node p.
6.	End of Enqueue Operation
 
Program:
```
struct Node   
{  
int data;  
struct Node *next;  
}*head;
void push(int data)  
{  
    struct Node* n = (struct Node*)malloc(sizeof(struct Node));
    n->data = data;
    n->next = head;
    head = n;
}
```
Output:

![image](https://github.com/user-attachments/assets/74f2b37d-5232-4560-81bd-f6118dea457f)

Result:
Thus, the program to insert elements in queue using linked list is verified successfully.



EXP NO:30 C FUNCTION TO FIND THE PEEK OF QUEUE USING LINKED LIST.


Aim:

The aim of this function is to retrieve the "peek" (the front element) of a queue implemented using a linked list

Algorithm:

1.	Check if the queue is empty:
o	If the queue is empty (i.e., the front pointer is NULL), return an error or a message indicating that the queue is empty.
2.	Access the front element:
o	If the queue is not empty, return the data stored in the front node of the linked list (i.e., the element at the head of the queue).

Program:
```
struct Node
{
   int data;
   struct Node *next;
}*front=NULL,*rear=NULL;
void peek()
{
    printf("%d",front->data);
}
```
Output:

![image](https://github.com/user-attachments/assets/a7c63b14-2e7a-4793-9aa0-9f35507ca340)

Result:

Thus, the program to retrieve the "peek" (the front element) of a queue implemented using a linked list is verified successfully.
