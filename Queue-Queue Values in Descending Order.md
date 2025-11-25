# Queue-Queue Values in Descending Order Using Python 🧮

This Python program simulates a queue using a list, removes the first two elements (FIFO order), and displays the remaining values in descending order.

## 🎯 Aim

To write a Python program to:
- Accept user inputs into a list (queue)
- Remove the first two elements (simulating dequeue)
- Display the remaining values in **descending order**

## 🧠 Algorithm

1. Create an empty list `q`.
2. Read an integer `n` to determine how many elements will be added.
3. Loop `n` times:
   - Read an input value.
   - Append it to the list `q`.
4. Remove the first element using `pop(0)`.
5. Remove the second element using `pop(0)` again.
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
