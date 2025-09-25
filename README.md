# Queue-implementation-in-cpp-
# C++ Queue Implementation using Arrays  

This repository contains a simple C++ program demonstrating a **queue** data structure using arrays.  

---

## What is a Queue?  
A **queue** is a linear data structure that follows the **FIFO (First In, First Out)** principle.  
- **Enqueue**: Insert element at the rear of the queue  
- **Dequeue**: Remove element from the front of the queue  
- **Front/Rear**: Pointers used to track the start and end of the queue

- Example 

<img width="683" height="203" alt="image" src="https://github.com/user-attachments/assets/d3f8c383-3c21-41e0-9466-33d7e17a45f7" />

<img width="683" height="236" alt="image" src="https://github.com/user-attachments/assets/bd835062-860b-4687-877c-6534c85657fe" />

<img width="683" height="204" alt="image" src="https://github.com/user-attachments/assets/a13aeda8-5ab0-41d1-a87e-a37ee82bc317" />






---

## Program Overview  

| Feature | Description |
|---------|-------------|
| Class | `Queue` with array of fixed size (`SIZE = 5`) |
| Operations | `enqueue(value)` – insert element<br>`dequeue()` – remove element<br>`display()` – show current queue elements |
| Front & Rear | `front` points to first element, `rear` points to last element in queue |
| Overflow & Underflow | Handles queue overflow and underflow situations with messages |

---

## Algorithm  

1. **Initialization:**  
   - Set `front = -1`, `rear = -1`  
   - Create array `arr[SIZE]` to store elements  

2. **Enqueue Operation:**  
   - If `rear == SIZE-1`, print "Queue Overflow"  
   - If first insertion (`front == -1`), set `front = 0`  
   - Increment `rear` and insert `value`  

3. **Dequeue Operation:**  
   - If `front == -1` or `front > rear`, print "Queue Underflow"  
   - Print and remove `arr[front]`  
   - Increment `front`  

4. **Display Operation:**  
   - If queue is empty, print "Queue is empty"  
   - Else, loop from `front` to `rear` and print elements  

5. **Main Function:**  
   - Create a `Queue` object  
   - Perform enqueue, dequeue, and display operations to demonstrate functionality  

---

## Concepts Demonstrated  
- Array-based queue implementation in C++  
- Queue operations: enqueue, dequeue, display  
- Handling of overflow and underflow  
- Use of class, private members, and methods  
