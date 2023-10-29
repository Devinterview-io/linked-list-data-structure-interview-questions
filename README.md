# ⚫ Linked Lists in Tech Interviews 2024: 31 Must-Know Questions & Answers

**Linked Lists** are linear data structures where elements are stored in nodes, and each node points to the next node in the sequence. Unlike arrays, they allow for efficient insertions and deletions in the middle of the list. In coding interviews, questions about linked lists test a candidate's grasp on **pointer manipulation** and understanding of **sequential data storage**.

Check out our carefully selected list of **basic** and **advanced** Linked Lists questions and answers to be well-prepared for your tech interviews in 2024.

![Linked Lists Decorative Image](https://storage.googleapis.com/dev-stack-app.appspot.com/blogImg/linkedLists.png?GoogleAccessId=firebase-adminsdk-bgeaf%40dev-stack-app.iam.gserviceaccount.com&Expires=1698606297&Signature=akC9z1kUeBAHKM0LlapWAQ72dXGoFBk4eiUyOlhwMF0pnPtTkkZpuApZc8yELaF16Sew34%2FfbpzOpczbQSBFqY2IPHB5QNpA5oqbEvWqOnT1IybvZBPD0LHxQO3pkt4HNX3aD1tKQ5umJlyIejWm4xpc6vFhL7EnfAfpsb%2B6pasDhECpwmt1GcYsl8%2FqMdK7tMOoEbIeX8Gqi47DqrtVSmmxtfQJ9O5rp1GutlpunTYrw2gzxiqJLQsoS6VyizCHxoRmReCJSeEvl2XOdIXI6KfR8BG66QwISLsGupn6PhY8Dcg9lsjR85JzbMQfP0vWLsxQyLyzX99bvKYQYWDKyQ%3D%3D)

👉🏼 You can also find all answers here: [Devinterview.io - Linked Lists](https://devinterview.io/data/linkedLists-interview-questions)

---

## 🔹 1. What is a _Linked List_?

### Answer

A **Linked List** is a dynamic data structure ideal for fast insertions and deletions. Unlike arrays, its elements aren't stored contiguously but are linked via pointers.

### Anatomy of a Linked List

A Linked List is a collection of **nodes**, each having:
- **Data**: The stored value.
- **Next Pointer**: A reference to the next node.

The list starts with a **Head** node and ends with a node having a **null** `Next` pointer.

### Visual Representation

![Linked List](https://firebasestorage.googleapis.com/v0/b/dev-stack-app.appspot.com/o/linked-lists%2Fsingly-linked-list.svg?alt=media&token=c6e2ad4f-e2d4-4977-a215-6253e71b6040)

### Key Features

- **Dynamic Size**: Adapts to data volume.
- **Non-Contiguous Memory**: Flexibility in storage.
- **Fast Insertions/Deletions**: Limited pointer adjustments needed.

### Types of Linked Lists

1. **Singly Linked List**: Each node has a single pointer to the next node. Traversal is unidirectional: from head to tail.
![Singly Linked List](https://firebasestorage.googleapis.com/v0/b/dev-stack-app.appspot.com/o/linked-lists%2Fsingly-linked-list.svg?alt=media&token=c6e2ad4f-e2d4-4977-a215-6253e71b6040)
2. **Doubly Linked List**: Each node have two pointers: one pointing to the next node and another to the previous node. This allows for bidirectional traversal.
![Doubly Linked List](https://firebasestorage.googleapis.com/v0/b/dev-stack-app.appspot.com/o/linked-lists%2Fdoubly-linked-list.svg?alt=media&token=5e14dad3-c42a-43aa-99ff-940ab1d9cc3d)
3. **Circular Linked List**: Like a singly linked list, but the tail node points back to the head, forming a loop.
![Circular Linked List](https://firebasestorage.googleapis.com/v0/b/dev-stack-app.appspot.com/o/linked-lists%2Fcircular-linked-list.svg?alt=media&token=b3b96bc7-3b16-4d07-978f-e4774a048ee1)
4. **Multi-level Linked List**: This specialized type has nodes with multiple pointers, each pointing to different nodes. It's often used in advanced data structures like multi-level caches.
![Multi-level Linked List](https://firebasestorage.googleapis.com/v0/b/dev-stack-app.appspot.com/o/linked-lists%2Fmulti-level-linked-list.svg?alt=media&token=967af5cf-8a95-4c05-a8fe-fb70f2b7ea57)

### Common Operations and Time Complexity

- **Traversal**: Scan through nodes — $O(n)$.
- **Insertion at the Beginning**: Add a node at the start — $O(1)$.
- **Insertion (other cases)/Deletion**: Add or remove nodes elsewhere in the list — $O(n)$.
- **Search**: Locate specific nodes — $O(n)$.
- **Sorting**: Order or organize nodes in the list. Commonly-used algorithms for linked lists like merge sort have a time complexity of $O(n \log n)$.
- **Merging**: Combine two lists — $O(n)$ where $n$ is the total number of nodes in both lists.
- **Reversal**: Flip node order — $O(n)$.

### Code Example: Singly Linked List

Here is the Python code:

```python
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None

class LinkedList:
    def __init__(self):
        self.head = None

    def insert(self, data):
        new_node = Node(data)
        if not self.head:
            self.head = new_node
        else:
            last_node = self.head
            while last_node.next:
                last_node = last_node.next
            last_node.next = new_node

    def display(self):
        current = self.head
        while current:
            print(current.data)
            current = current.next

# Usage
my_list = LinkedList()
my_list.insert(1)
my_list.insert(2)
my_list.insert(3)
my_list.display()

# Output:
# 1
# 2
# 3
```

---

## 🔹 2. What are some real-life _Use Cases_ of _Linked Lists_?

### Answer

**Linked lists** are widely used in real-world applications for their advantages in dynamic memory management and data manipulation.

### Practical Applications

#### Operating Systems

- **Task Scheduling**: Linked lists efficiently manage queues of tasks awaiting execution.
- **Memory Management**: They facilitate dynamic memory allocation, especially useful in applications like memory pool management.

#### Text Editors

- **Undo/Redo Functionality**: Editors maintain a stack of changes using linked lists, enabling the undo and redo functionalities.

#### Music Players

- **Playlists**: Linked lists offer flexibility in managing playlists, allowing for the easy addition, deletion, and navigation of tracks.

#### Web Browsers

- **Browser History**: Linked lists, especially doubly linked ones, are instrumental in navigating web page histories, permitting both forward and backward traversal.

#### Compilers

- **Symbol Tables**: Compilers employ linked lists to manage tables containing variable and function identifiers. This provides scoped access to these identifiers during different stages of compilation.

#### Database Management Systems

- **Transient Storage Structures**: While core storage might use trees or hash indexes, linked lists can serve auxiliary roles, especially in in-memory databases.

#### Artificial Intelligence and Machine Learning

- **Graph Representation**: Algorithms requiring graph representations often utilize adjacency lists, essentially arrays of linked lists, to depict vertices and edges.

#### Caching Algorithms

- **LRU Cache**: Linked lists, particularly doubly linked ones, play a pivotal role in the Least Recently Used (LRU) caching algorithms to determine which items to replace.

#### Networking

- **Packet Management**: In networking scenarios, linked lists help manage queues of data packets awaiting transmission.

#### Gaming

- **Character Inventory**: In role-playing games, a character's inventory, where items are added and removed frequently, can be managed using linked lists.

---

## 🔹 3. What are some pros and cons of _Linked List_ compared to _Arrays_?

### Answer

Let's look at the pros and cons of using **linked lists** compared to **arrays**.

### Advantages of Linked Lists

- **Dynamic Size**: Linked lists naturally adjust to changing sizes, while arrays are fixed-sized. Dynamic arrays auto-resize but can lag in efficiency during frequent mid-list insertions or deletions.

- **Efficient Insertions/Deletions**: Insertions and deletions in linked lists only require a few pointer adjustments, whereas arrays may need shifting of elements.

- **Flexibility in Size**: Memory for nodes in linked lists is allocated or released as needed, potentially reducing memory wastage.

- **Merging and Splitting**: It's simpler to merge or split linked lists.

### Disadvantages of Linked Lists

- **Memory Overhead**: Each node has overhead due to data and a pointer, using more memory than arrays for the same number of elements.

- **Sequential Access**: Linked lists only allow sequential access, unlike arrays that support direct indexing.

- **Cache Inefficiency**: Nodes might be scattered in memory, leading to cache misses.

- **No Random Access**: Element retrieval might require full list traversal, whereas arrays offer constant-time access.

- **Data Integrity**: If a node's link breaks, subsequent nodes are lost.

- **Search Efficiency**: Requires linear scans, which can be slower than searches in sorted arrays or trees.

- **Sorting**: Certain sorting algorithms, like QuickSort, are less efficient with linked lists than with arrays.


---

## 🔹 4. When is _Doubly Linked List_ more efficient than _Singly Linked List_?

### Answer

**Doubly linked lists** offer advantages in specific use-cases but use more memory and may require more complex thread-safety

### Key Efficiency Differences

- **Deletion**: If only the node to be deleted is known, doubly linked lists can delete it in $O(1)$ time, whereas singly linked lists may take up to $O(n)$ to find the prior node.

- **Tail Operations**: In doubly linked lists, tail-related tasks are $O(1)$. For singly linked lists without a tail pointer, these are $O(n)$.

### Practical Use-Cases

- **Cache Implementations**: Doubly linked lists are ideal due to quick bidirectional insertion and deletion.

- **Text Editors and Undo/Redo**: The bidirectional capabilities make doubly linked lists more efficient for these functions.

---

## 🔹 5. Compare _Array-based_ vs _Linked List_ stack implementations.

### Answer

**Array-based stacks** excel in time efficiency and direct element access. In contrast, **linked list stacks** are preferable for dynamic sizing and easy insertions or deletions.

### Common Features

- **Speed of Operations**: Both `pop` and `push` are $O(1)$ operations.
- **Memory Use**: Both have $O(n)$ space complexity.
- **Flexibility**: Both can adapt their sizes, but their resizing strategies differ.

### Key Distinctions

#### Array-Based Stack

- **Locality**: Consecutive memory locations benefit CPU caching.
- **Random Access**: Provides direct element access.
- **Iterator Needs**: Preferable if indexing or iterators are required.
- **Performance**: Slightly faster for top-element operations and potentially better for time-sensitive tasks due to caching.
- **Push**: $O(1)$ on average; resizing might cause occasional $O(n)$.

#### Linked List Stack

- **Memory Efficiency**: Better suited for fluctuating sizes and limited memory scenarios.
- **Resizing Overhead**: No resizing overheads.
- **Pointer Overhead**: Requires extra memory for storing pointers.

### Code Example: Array-Based Stack

Here is the Python code:

```python
class ArrayBasedStack:
    def __init__(self):
        self.stack = []
    def push(self, item):
        self.stack.append(item)
    def pop(self):
        return self.stack.pop() if self.stack else None
```

### Code Example: Linked List Stack

Here is the Python code:

```python
class Node:
    def __init__(self, data=None):
        self.data = data
        self.next = None
class LinkedListStack:
    def __init__(self):
        self.head = None
    def push(self, item):
        new_node = Node(item)
        new_node.next = self.head
        self.head = new_node
    def pop(self):
        if self.head:
            temp = self.head
            self.head = self.head.next
            return temp.data
        return None
```

---

## 🔹 6. When is a _Circular Linked List_ useful?

### Answer

A **circular Linked List** is a specific type of linked list where the tail node is intentionally connected back to the head node to form a closed loop.

![Circular Linked List](https://firebasestorage.googleapis.com/v0/b/dev-stack-app.appspot.com/o/linked-lists%2Fcircular-linked-list.svg?alt=media&token=b3b96bc7-3b16-4d07-978f-e4774a048ee1)

### Common Use Cases

- **Emulating Circular Structures**: Useful for representing naturally circular data like polygon vertices, buffer pools, or round-robin scheduling in operating systems.
  
- **Queue Efficiency**: Accessing the front and rear elements in constant time, improving queue implementations.

- **Algorithmic Simplifications**: Enables easier data manipulations like list splitting and concatenation in constant time.

### Code Example: Queue Efficiency

Here is the Python code:

```python
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None

class CircularQueue:
    def __init__(self):
        self.front = self.rear = None

    def enqueue(self, data):
        new_node = Node(data)
        if self.rear:
            self.rear.next, self.rear = new_node, new_node
        else:
            self.front = self.rear = new_node
        self.rear.next = self.front

    def dequeue(self):
        if not self.front: return None
        if self.front == self.rear: self.front = self.rear = None
        else: self.front = self.front.next; self.rear.next = self.front
        return self.front.data if self.front else None

# Example usage:
cq = CircularQueue()
cq.enqueue(1); cq.enqueue(2); cq.enqueue(3)
print(cq.dequeue(), cq.dequeue(), cq.dequeue(), cq.dequeue())
```

---

## 🔹 7. Why is _Merge Sort_ preferred over _QuickSort_ for sorting _Linked Lists_?

### Answer

While both **QuickSort** and **MergeSort** are powerful sorting algorithms, MergeSort is often favored for linked lists for a variety of reasons, including its stability and optimized disk I/O operations.

### Advantages of MergeSort for Linked Lists

- **No Need for Random Access**: Unlike QuickSort, which benefits from direct access to elements for efficient partitioning, MergeSort doesn't require random access, making it ideal for linked lists.
  
- **Cache Efficiency**: MergeSort sequentially accesses elements, optimizing CPU cache usage, especially with large data sets.

- **Optimized Disk Operations**: MergeSort performs fewer disk I/O operations when sorting data that doesn't fit in memory, outperforming QuickSort in such scenarios.

### Code Example: MergeSort on Linked List

Here is the Python code:

```python
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None

def merge_sort(head):
    if not head or not head.next:
        return head
    
    mid = get_middle(head)
    next_to_mid = mid.next
    mid.next = None
    
    left = merge_sort(head)
    right = merge_sort(next_to_mid)
    
    return merge(left, right)

def get_middle(head):
    slow, fast = head, head
    while fast.next and fast.next.next:
        slow, fast = slow.next, fast.next.next
    return slow

def merge(left, right):
    dummy = Node(0)
    curr = dummy
    
    while left and right:
        if left.data < right.data:
            curr.next, left = left, left.next
        else:
            curr.next, right = right, right.next
        curr = curr.next
    
    curr.next = left or right
    return dummy.next
```

---

## 🔹 8. Is it possible to _Traverse a Linked List_ in _O(n1/2)_? (Jump Pointers).

### Answer

While it may not be possible to **traverse a linked list** in better than $O(n)$ time complexity in the strictest sense, there are techniques that can make the traversal process more efficient in certain contexts.

In particular, let's explore the idea of "**Jump Pointers**" or "**Square Root Jumps**" which allows you to traverse a linked list in $O(\sqrt{n})$ time complexity.

### What Are Jump Pointers?

**Jump Pointers** allow for quicker traversal by "jumping" over a fixed number of nodes $k$ during each step. This reduces the total number of nodes visited, thereby improving the time complexity.

For instance, when $k = \sqrt{n}$, the traversal time complexity drops to $O(\sqrt{n})$.

### Code Example: Jump Pointers

Here is the Python code:

```python
# Node definition
class Node:
    def __init__(self, data=None):
        self.data = data
        self.next = None

# LinkedList definition
class LinkedList:
    def __init__(self):
        self.head = None

    # Add node to end
    def append(self, data):
        new_node = Node(data)
        if not self.head:
            self.head = new_node
            return
        last = self.head
        while last.next:
            last = last.next
        last.next = new_node

    # Traverse using Jump Pointers
    def jump_traverse(self, jump_size):
        current = self.head
        while current:
            print(current.data)
            for _ in range(jump_size):
                if not current:
                    return
                current = current.next

# Create linked list and populate it
llist = LinkedList()
for i in range(1, 11):
    llist.append(i)

# Traverse using Jump Pointers
print("Jump Pointer Traversal:")
llist.jump_traverse(int(10**0.5))
```

---

## 🔹 9. How to apply _Binary Search_ in _O(log n)_ on a _Sorted Linked List_? (Skip Lists).

### Answer

While **Binary Search** boasts a time complexity of $O(\log n)$, applying it to a singly linked list is less straightforward due to the list's linear nature and $O(n)$ access time. However, **Skip Lists** offer a clever workaround to achieve sub-linear search times in linked lists.

### Why Traditional Binary Search Falls Short in Linked Lists

In a **singly linked list**, random access to elements is not possible. To reach the $k$-th element, you have to traverse $k-1$ preceding nodes. Therefore, the act of **accessing a middle element** during binary search incurs a time complexity of $O(n)$.

### Skip Lists: A Solution for Sub-linear Search

Skip Lists augment sorted linked lists with multiple layers of '**express lanes**', allowing you to leapfrog over sections of the list. Each layer contains a subset of the elements from the layer below it, enabling faster search.

![Skip List Example](https://upload.wikimedia.org/wikipedia/commons/thumb/8/86/Skip_list.svg/1920px-Skip_list.svg.png)

By starting at the topmost layer and working downwards, you can **reduce the search space** at each step. This results in an average time complexity of $O(\log n)$ for search operations.

### Code Example: Visualizing a Skip List

Here is the Python code:

```python
# Define a node for the Skip List
class SkipNode:
    def __init__(self, value):
        self.value = value
        self.next = []

# Initialize a Skip List
class SkipList:
    def __init__(self):
        self.head = SkipNode(float('-inf'))  # Initialize with the smallest possible value
        self.levels = 1  # Start with a single level
```

---
## 🔹 10. Is it possible to do _Binary Search_ on a _Doubly Linked List_ in _O(n)_ time?

### Answer

👉🏼 Check out all 31 answers here: [Devinterview.io - Linked Lists](https://devinterview.io/data/linkedLists-interview-questions)

---

## 🔹 11. Explain _Floyd's Cycle Detection Algorithm_.

### Answer

👉🏼 Check out all 31 answers here: [Devinterview.io - Linked Lists](https://devinterview.io/data/linkedLists-interview-questions)

---

## 🔹 12. Is there an algorithm _Better Than Floyd's_ for _Cycle Detection_ in linked lists?

### Answer

👉🏼 Check out all 31 answers here: [Devinterview.io - Linked Lists](https://devinterview.io/data/linkedLists-interview-questions)

---

## 🔹 13. Implement a _Linked List_ using _Stack_.

### Answer

👉🏼 Check out all 31 answers here: [Devinterview.io - Linked Lists](https://devinterview.io/data/linkedLists-interview-questions)

---

## 🔹 14. Reverse a _Singly Linked List_ using only _Two Pointers_.

### Answer

👉🏼 Check out all 31 answers here: [Devinterview.io - Linked Lists](https://devinterview.io/data/linkedLists-interview-questions)

---

## 🔹 15. Convert a _Singly Linked List_ to a _Circular Linked List_.

### Answer

👉🏼 Check out all 31 answers here: [Devinterview.io - Linked Lists](https://devinterview.io/data/linkedLists-interview-questions)

---

## 🔹 16. Convert a _Singly Linked List_ to a _Doubly Linked List_.

### Answer

👉🏼 Check out all 31 answers here: [Devinterview.io - Linked Lists](https://devinterview.io/data/linkedLists-interview-questions)

---

## 🔹 17. _Insert_ an item in a _Sorted Linked List_, while maintaining order.

### Answer

👉🏼 Check out all 31 answers here: [Devinterview.io - Linked Lists](https://devinterview.io/data/linkedLists-interview-questions)

---

## 🔹 18. Detect if a _List_ is _Cyclic_ using _Hash Table_.

### Answer

👉🏼 Check out all 31 answers here: [Devinterview.io - Linked Lists](https://devinterview.io/data/linkedLists-interview-questions)

---

## 🔹 19. Merge two sorted Singly Linked Lists without creating new nodes.

### Answer

👉🏼 Check out all 31 answers here: [Devinterview.io - Linked Lists](https://devinterview.io/data/linkedLists-interview-questions)

---

## 🔹 20. _Find the N-th element_ from the end of a _Singly Linked List_.

### Answer

👉🏼 Check out all 31 answers here: [Devinterview.io - Linked Lists](https://devinterview.io/data/linkedLists-interview-questions)

---

## 🔹 21. Implement _Doubly Linked List_ using _Stacks_ with minimal complexity.

### Answer

👉🏼 Check out all 31 answers here: [Devinterview.io - Linked Lists](https://devinterview.io/data/linkedLists-interview-questions)

---

## 🔹 22. Convert a _Binary Tree_ into a _Doubly Linked List_.

### Answer

👉🏼 Check out all 31 answers here: [Devinterview.io - Linked Lists](https://devinterview.io/data/linkedLists-interview-questions)

---

## 🔹 23. Remove _Duplicates_ from an _Unsorted Linked List_.

### Answer

👉🏼 Check out all 31 answers here: [Devinterview.io - Linked Lists](https://devinterview.io/data/linkedLists-interview-questions)

---

## 🔹 24. Find _Common Elements_ in two given _Linked Lists_ and return them as a new _Linked List_.

### Answer

👉🏼 Check out all 31 answers here: [Devinterview.io - Linked Lists](https://devinterview.io/data/linkedLists-interview-questions)

---

## 🔹 25. _Split_ the _Linked List_ into _k_ consecutive parts.

### Answer

👉🏼 Check out all 31 answers here: [Devinterview.io - Linked Lists](https://devinterview.io/data/linkedLists-interview-questions)

---

## 🔹 26. _Sum_ two numbers represented as _Linked Lists_.

### Answer

👉🏼 Check out all 31 answers here: [Devinterview.io - Linked Lists](https://devinterview.io/data/linkedLists-interview-questions)

---

## 🔹 27. _Reverse_ a _Linked List_ recursively.

### Answer

👉🏼 Check out all 31 answers here: [Devinterview.io - Linked Lists](https://devinterview.io/data/linkedLists-interview-questions)

---

## 🔹 28. Find a _Merge Point_ (Intersection) of two _Linked Lists_.

### Answer

👉🏼 Check out all 31 answers here: [Devinterview.io - Linked Lists](https://devinterview.io/data/linkedLists-interview-questions)

---

## 🔹 29. Given a _Singly Linked List_, determine if it is a _Palindrome_.

### Answer

👉🏼 Check out all 31 answers here: [Devinterview.io - Linked Lists](https://devinterview.io/data/linkedLists-interview-questions)

---

## 🔹 30. Find the length of a _Linked List_ that contains a _Cycle_.

### Answer

👉🏼 Check out all 31 answers here: [Devinterview.io - Linked Lists](https://devinterview.io/data/linkedLists-interview-questions)

---

## 🔹 31. _Duplicate_ a _Linked List_ with _Random Pointers_ using _O(1)_ space.

### Answer

👉🏼 Check out all 31 answers here: [Devinterview.io - Linked Lists](https://devinterview.io/data/linkedLists-interview-questions)

---

