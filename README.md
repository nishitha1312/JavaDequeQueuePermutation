# Deque and Randomized Queue Implementation

This Java project implements two fundamental data structures: **Deque** (double-ended queue) and **Randomized Queue**, along with a simple **Permutation generator**. Both are implemented from scratch with full iterator support and robust exception handling.

---

## Features

### Deque
- Supports adding and removing items from both **front** and **back** in constant time.
- Supports **iteration** from front to back.
- Throws exceptions for invalid operations (e.g., adding null or removing from empty deque).
- Fully generic implementation: works with any object type.

**API Methods:**
- `addFirst(Item item)` — add an item to the front.
- `addLast(Item item)` — add an item to the back.
- `removeFirst()` — remove and return item from front.
- `removeLast()` — remove and return item from back.
- `isEmpty()` — check if deque is empty.
- `size()` — number of items in deque.
- `iterator()` — iterate from front to back.

---

### RandomizedQueue
- Queue where **items are removed uniformly at random**.
- Supports **enqueue**, **dequeue**, and **sample** operations.
- Independent iterator returns items in **random order**.
- Resizable array implementation ensures **amortized constant time** operations.

**API Methods:**
- `enqueue(Item item)` — add an item to the queue.
- `dequeue()` — remove and return a random item.
- `sample()` — return a random item without removing it.
- `isEmpty()` — check if queue is empty.
- `size()` — number of items in the queue.
- `iterator()` — iterate items in random order.

---

### Permutation
- Uses **RandomizedQueue** to generate a random permutation of input strings.
- Reads input from **standard input** and prints a fixed number of random items.
- Example usage: `java Permutation 3` (prints 3 random items from input).

---

## Requirements

- Java 8 or higher
- [Princeton Algorithms library](https://algs4.cs.princeton.edu/code/) (for `StdIn`, `StdOut`, and `StdRandom`)

---
