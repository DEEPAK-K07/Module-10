# Queue-Queue Values in Descending Order Using Python 🧮

This Python program simulates a queue using a list, removes the first two elements (FIFO order), and displays the remaining values in descending order.

## 🎯 Aim

To write a Python program to:
- Accept user inputs into a list (queue)
- Remove the first two elements (simulating dequeue)
- Display the remaining values in *descending order*

## 🧠 Algorithm

1. Create an empty list q.
2. Read an integer n to determine how many elements will be added.
3. Loop n times:
   - Read an input value.
   - Append it to the list q.
4. Remove the first element using pop(0).
5. Remove the second element using pop(0) again.
6. Sort the list in descending order.
7. Print the updated list.

## 🧪 Program: 
```
from collections import deque

# Read 5 strings
q = deque()
for _ in range(5):
    q.append(input().strip())

# Sort in descending order
sorted_list = sorted(q, reverse=True)

# Print space-separated
print(' '.join(sorted_list))
```
### Output:
![image](https://github.com/user-attachments/assets/962cf037-4b35-4b74-a417-3ed5d4fb0adb)

## Result:
      Thus Python program simulates a queue using a list, removes the first two elements (FIFO order), and displays the remaining values in descending order is successfully executed.# Queue-Queue Values in Descending Order Using Python 🧮

This Python program simulates a queue using a list, removes the first two elements (FIFO order), and displays the remaining values in descending order.

## 🎯 Aim

To write a Python program to:
- Accept user inputs into a list (queue)
- Remove the first two elements (simulating dequeue)
- Display the remaining values in *descending order*

## 🧠 Algorithm

1. Create an empty list q.
2. Read an integer n to determine how many elements will be added.
3. Loop n times:
   - Read an input value.
   - Append it to the list q.
4. Remove the first element using pop(0).
5. Remove the second element using pop(0) again.
6. Sort the list in descending order.
7. Print the updated list.

## 🧪 Program: 
```
from collections import deque

# Read 5 strings
q = deque()
for _ in range(5):
    q.append(input().strip())

# Sort in descending order
sorted_list = sorted(q, reverse=True)

# Print space-separated
print(' '.join(sorted_list))
```
### Output:
![image](https://github.com/user-attachments/assets/962cf037-4b35-4b74-a417-3ed5d4fb0adb)

## Result:
      Thus Python program simulates a queue using a list, removes the first two elements (FIFO order), and displays the remaining values in descending order is successfully executed.

# Queue-Remove Two String Values from the Rear End in Python 🧵

This Python program demonstrates how to manage a list of strings and remove the last two elements (i.e., from the rear of the list).

## 🎯 Aim

To write a Python program to:
- Accept n string values from the user
- Remove the last two values (rear end of the list)
- Display the updated list

## 🧠 Algorithm

1. Create an empty list q.
2. Read an integer n from the user (number of strings).
3. Loop n times:
   - Read a string input.
   - Append it to the list q.
4. Remove the last element using pop().
5. Remove the next last element using pop() again.
6. Display the updated list.

##  Program:
```
  q = []
  n=int(input())
  for i in range(n):
     q.append(input())
  q.pop(0)
  q.pop(0)
  print(q)
```

### Output:
![image](https://github.com/user-attachments/assets/f973912c-841d-42da-9bdf-c384572c1bea)


## Result:
Thus, the program has been execueted successfully.

# Stack Implementation Using LifoQueue (Max Size 7) 🔄

This Python program demonstrates a stack implemented using the LifoQueue class from the queue module. It allows up to 7 elements, checks if the stack is full, and then prints the elements in reverse (LIFO) order.

## 🎯 Aim

To create a Python program that:
- Implements a stack using LifoQueue with a maximum size of 7
- Adds user-inputted values to the stack
- Checks whether the stack is full
- Prints the stack elements in reverse order (LIFO)

## 📋 Algorithm

1. Import the LifoQueue class from the queue module.
2. Create a stack with a maximum size of 7.
3. Read the number of elements (n) to be added to the stack.
4. Loop n times:
   - Read a value from the user.
   - Use put() to push it onto the stack if it's not full.
5. Use full() to check if the stack is full and print the result.
6. Use get() repeatedly to pop and print elements in reverse order.

## Program
```
  from queue import LifoQueue
  stack = LifoQueue(maxsize=7)
  n= int(input())
  for i in range(n):
      stack.put(input())
  print(stack.full())
  for i in range(n):
      print(stack.get())
```

## 🧪 Sample Input and Output
![image](https://github.com/user-attachments/assets/05e20587-542b-4fd4-9943-f0f13e78aebf)

## Result:
Thus, the program has been execueted successfully.

# # Stack-Stack Reversal Program 🔁

This Python program demonstrates how to reverse the values in a stack using basic stack operations like push and pop.

## 🎯 Aim

To write a Python program that reverses the values in a stack using standard stack operations.

## 📋 Algorithm

1. Create an empty stack.
2. Read an integer n from the user (number of elements to push).
3. Loop n times:
   - Read an integer from the user.
   - Push it onto the stack.
4. Create an empty list called reverse.
5. While the stack is not empty:
   - Pop the top element.
   - Append it to reverse.
6. Print the reversed list.


### Program:
```
  stack = []
  n=int(input())
  for i in range(n):
     value=int(input())
     stack.append(value)
  reverse= []
  while stack:
     reverse.append(stack.pop())
  print(reverse)
```
## 🧪 Sample Input and Output
![image](https://github.com/user-attachments/assets/8bf53030-a254-493f-ae95-7021114c9c9e)

## Result
Thus, the program has been execueted successfully.

# 🔄 Types of Queue-Circular Queue in Python

This project demonstrates the implementation of a *Circular Queue* in Python. The queue accepts 3 user values, performs enqueue and dequeue operations, and displays the removed values.

---

## 🎯 Aim

To develop a Python program that implements a Circular Queue:
- Accepts 3 values from the user
- Removes the 3 values from the queue
- Displays the removed values

---

## 🧠 Algorithm

1. *Initialize* a circular queue of fixed size (e.g., 5).
2. *Define the following functions*:
   - enqueue(): Inserts an element into the queue.
   - dequeue(): Removes an element from the queue.
   - display(): Shows the queue contents.
3. Accept 3 values from the user using the enqueue() method.
4. Remove 3 values using the dequeue() method.
5. Print the removed values.

---

## 💻 Program:

  class MyCircularQueue():
      def __init__(self, k):
          self.k = k
          self.queue = [None] * k
          self.head = self.tail = -1
      def enqueue(self, data):
          if ((self.tail+1)%self.k==self.head):
              print("The circular queue is full")
          elif (self.head==-1):
              self.head=0
              self.tail=0
              self.queue[self.tail]=data
          else:
              self.tail=(self.tail+1)%self.k
              self.queue[self.tail]=data
      
      def printCQueue(self):
          if(self.head==-1):
              print("No element in the circular queue")
          elif (self.tail>=self.head):
              for i in range(self.head,self.tail+1):
                  print(self.queue[i],end=' ')
              print()
          else:
              for i in range(self.head,self.k):
                  print(self.queue[i],end=' ')
              for i in range(0,self.tail+1):
                  print(self.queue[i],end=' ')
              print()
  obj = MyCircularQueue(5)
  for i in range(5):
      obj.enqueue(int(input()))
  obj.printCQueue()

### Output:
![image](https://github.com/user-attachments/assets/f933814a-7651-4405-9910-b7faba1cb4f7)

## Result:
Thus, the program has been execueted successfully.
