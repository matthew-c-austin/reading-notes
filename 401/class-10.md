# Stacks and Queues Cheatsheet

## 1. Stacks

### A. Definition

- A stack is a linear data structure that follows the **Last In First Out (LIFO)** principle.
- Items are added and removed only from the top of the stack.
- Main operations: _push_, _pop_, and _peek_.

### B. Terminology

- **Top**: The top element of the stack.
- **Push**: Adds an element to the top of the stack.
- **Pop**: Removes the top element from the stack.
- **Peek**: Returns the value of the top element without removing it.
- **IsEmpty**: Checks if the stack is empty.

### C. Time Complexity

- Push: O(1)
- Pop: O(1)
- Peek: O(1)
- IsEmpty: O(1)

### D. Use Cases

- Reversing strings or numbers.
- Undo/redo functionality.
- Syntax checking in compilers.

## 2. Queues

### A. Definition

- A queue is a linear data structure that follows the **First In First Out (FIFO)** principle.
- Items are added at the end (rear) and removed from the front (head).
- Main operations: _enqueue_, _dequeue_, and _peek_.

### B. Terminology

- **Front**: The first element in the queue.
- **Rear**: The last element in the queue.
- **Enqueue**: Adds an element to the rear of the queue.
- **Dequeue**: Removes the front element from the queue.
- **Peek**: Returns the value of the front element without removing it.
- **IsEmpty**: Checks if the queue is empty.

### C. Time Complexity

- Enqueue: O(1)
- Dequeue: O(1)
- Peek: O(1)
- IsEmpty: O(1)

### D. Use Cases

- Task scheduling and prioritization.
- Data buffering.
- Managing processes in operating systems.

## 3. Variations

### A. Double-Ended Queue (Deque)

- Allows insertion and deletion at both ends (front and rear).
- Can function as both a stack and a queue.

### B. Priority Queue

- Each element is associated with a priority.
- Elements are dequeued based on their priority values.

### C. Circular Queue

- Rear and front pointers wrap around to the first element when the end is reached.
- Efficient use of memory.
