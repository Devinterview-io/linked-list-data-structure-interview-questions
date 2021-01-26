<div data-v-5e9078c0="">

# Top 43 Linked Lists interview questions and answers in 2021.

[![](https://source.unsplash.com/collection/52661698/700x350)](https://devinterview.io/)

You can check all 43 Linked Lists interview questions here 👉 https://devinterview.io/data/linkedLists-interview-questions

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 1\. Name some advantages of Linked List

</div>

<div>

### Answer:

<div class="answer">

<div>

<div>

<div class="AnswerBody">

There are some:

*   Linked Lists are **Dynamic Data Structure** - it can grow and shrink at runtime by allocating and deallocating memory. So there is no need to give initial size of linked list.
*   Insertion and Deletion are **simple to implement** - Unlike array here we don’t have to shift elements after insertion or deletion of an element. In linked list we just have to update the address present in next pointer of a node.
*   **Efficient Memory Allocation/No Memory Wastage** - In case of array there is lot of memory wastage, like if we declare an array of size 10 and store only 6 elements in it then space of 4 elements are wasted. There is no such problem in linked list as memory is allocated only when required.

</div>

</div>

<div class="row my-2">

<div><span>_Source:_ <span>[www.thecrazyprogrammer.com](https://www.thecrazyprogrammer.com/2016/11/advantages-disadvantages-linked-list.html "Name some advantages of Linked List Interview Questions Source To Answer")</span></span>   </div>

</div>

</div>

</div>

</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 2\. Define Linked List

</div>

<div>

### Answer:

<div class="answer">

<div>

<div>

<div class="AnswerBody">

A **linked list** is a linear data structure where each element is a separate object. Each element (we will call it a **node**) of a list is comprising of two items - the **data** and a **reference (pointer)** to the next node. The last node has a reference to **null**. The entry point into a linked list is called the **head** of the list. It should be noted that _head is not a separate node,_ but the reference to the first node. If the list is empty then the head is a null reference.

</div>

</div>

<div class="row my-2">

<div><span>_Source:_ <span>[www.cs.cmu.edu](https://www.cs.cmu.edu/~adamchik/15-121/lectures/Linked%20Lists/linked%20lists.html "Define Linked List Interview Questions Source To Answer")</span></span>   </div>

</div>

</div>

</div>

</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 3\. Name some disadvantages of Linked Lists?

</div>

<div>

### Answer:

<div class="answer">

<div>

<div>

<div class="AnswerBody">

Few disadvantages of linked lists are :

*   They use more memory than arrays because of the storage used by their pointers.
*   Difficulties arise in linked lists when it comes to reverse traversing. For instance, singly linked lists are cumbersome to navigate backwards and while doubly linked lists are somewhat easier to read, memory is wasted in allocating space for a back-pointer.
*   Nodes in a linked list must be read in order from the beginning as linked lists are inherently sequential access.
*   Random access has linear time.
*   Nodes are stored incontiguously (no or poor cache locality), greatly increasing the time required to access individual elements within the list, especially with a CPU cache.
*   If the link to list's node is accidentally destroyed then the chances of data loss after the destruction point is huge. Data recovery is not possible.
*   Search is linear versus logarithmic for sorted arrays and binary search trees.
*   Different amount of time is required to access each element.
*   Not easy to sort the elements stored in the linear linked list.

</div>

</div>

<div class="row my-2">

<div><span>_Source:_ <span>[www.quora.com](https://www.quora.com/What-are-the-disadvantages-of-linked-lists "Name some disadvantages of Linked Lists? Interview Questions Source To Answer")</span></span>   </div>

</div>

</div>

</div>

</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 4\. What is a cycle/loop in the singly-linked list?

</div>

<div>

### Answer:

<div class="answer">

<div>

<div>

<div class="AnswerBody">

A **cycle/loop** occurs when a node’s next points _back_ to a _previous node_ in the list. The linked list is no longer linear with a beginning and end—instead, it cycles through a loop of nodes.

</div>

</div>

<div class="row my-2">

<div><span>_Source:_ <span>[www.interviewcake.com](https://www.interviewcake.com/question/java/linked-list-cycles "What is a cycle/loop in the singly-linked list? Interview Questions Source To Answer")</span></span>   </div>

</div>

</div>

</div>

</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 5\. What are some types of Linked List?

</div>

<div>

### Answer:

<div class="answer">

<div>

<div>

<div class="AnswerBody">

*   A **singly linked list**

*   A **doubly linked list** is a list that has two references, one to the next node and another to previous node.

*   A **multiply linked list** - each node contains two or more link fields, each field being used to connect the same set of data records in a different order of same set(e.g., by name, by department, by date of birth, etc.).
*   A **circular linked list** - where last node of the list points back to the first node (or the head) of the list.

</div>

</div>

<div class="row my-2">

<div><span>_Source:_ <span>[www.cs.cmu.edu](https://www.cs.cmu.edu/~adamchik/15-121/lectures/Linked%20Lists/linked%20lists.html "What are some types of Linked List? Interview Questions Source To Answer")</span></span>   </div>

</div>

</div>

</div>

</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 6\. What is time complexity of Linked List operations?

</div>

<div>

### Answer:

<div class="answer">

<div>

<div>

<div class="AnswerBody">

*   A linked list can typically only be accessed via its head node. From there you can only traverse from node to node until you reach the node you seek. Thus **access is `_O_(_n_)`**.
*   Searching for a given value in a linked list similarly requires traversing all the elements until you find that value. Thus **search is `_O_(_n_)`**.
*   Inserting into a linked list requires re-pointing the previous node (the node before the insertion point) to the inserted node, and pointing the newly-inserted node to the next node. Thus **insertion is `_O_(_1_)`**.
*   Deleting from a linked list requires re-pointing the previous node (the node before the deleted node) to the next node (the node after the deleted node). Thus **deletion is `_O_(_1_)`**.

</div>

</div>

<div class="row my-2">

<div><span>_Source:_ <span>[github.com](https://github.com/tim-hr/stuff/wiki/Time-complexity:-linked-lists "What is time complexity of Linked List operations? Interview Questions Source To Answer")</span></span>   </div>

</div>

</div>

</div>

</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 7\. Under what circumstances are Linked Lists useful?

</div>

<div>

### Answer:

<div class="answer">

<div>

<div>

<div class="AnswerBody">

Linked lists are very useful when you need :

*   to do a lot of insertions and removals, but not too much searching, on a list of arbitrary (unknown at compile-time) length.
*   splitting and joining (bidirectionally-linked) lists is very efficient.
*   You can also combine linked lists - e.g. tree structures can be implemented as "vertical" linked lists (parent/child relationships) connecting together horizontal linked lists (siblings).

Using an array based list for these purposes has severe limitations:

*   Adding a new item means the array must be reallocated (or you must allocate more space than you need to allow for future growth and reduce the number of reallocations)
*   Removing items leaves wasted space or requires a reallocation
*   inserting items anywhere except the end involves (possibly reallocating and) copying lots of the data up one position

</div>

</div>

<div class="row my-2">

<div><span>_Source:_ <span>[stackoverflow.com](https://stackoverflow.com/questions/2429217/under-what-circumstances-are-linked-lists-useful "Under what circumstances are Linked Lists useful? Interview Questions Source To Answer")</span></span>   </div>

</div>

</div>

</div>

</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 8\. How to implement Linked List Using Stack?

</div>

<div>

### Answer:

<div class="answer">

<div>

<div>

<div class="AnswerBody">

You can simulate a linked list by using two stacks. One stack is the "list," and the other is used for temporary storage.

*   To **add** an item at the head, simply push the item onto the stack.
*   To **remove** from the head, pop from the stack.
*   To **insert** into the middle somewhere, pop items from the "list" stack and push them onto the temporary stack until you get to your insertion point. Push the new item onto the "list" stack, then pop from the temporary stack and push back onto the "list" stack. Deletion of an arbitrary node is similar.

This isn't terribly efficient, by the way, but it would in fact work.

</div>

</div>

<div class="row my-2">

<div><span>_Source:_ <span>[stackoverflow.com](https://stackoverflow.com/questions/36150565/how-to-implement-linked-list-using-stack "How to implement Linked List Using Stack? Interview Questions Source To Answer")</span></span>   </div>

</div>

</div>

</div>

</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 9\. How to reverse a singly Linked List using only two pointers?

</div>

<div>

### Answer:

<div class="answer">

<div>

<div>

<div class="AnswerBody">

Nothing faster than `_O_(_n_)` can be done. You need to traverse the list and alter pointers on every node, so time will be proportional to the number of elements.

</div>

</div>

<div style="font-size: 14px;">

<div class="mb-3 mt-2"><span class="h5">Implementation</span></div>

<div>

<nav class="mdc-tab-bar">

<div class="mdc-tab-scroller">

<div class="mdc-tab-scroller__scroll-area mdc-tab-scroller__scroll-area--scroll" style="margin-bottom: 0px;">

<div class="mdc-tab-scroller__scroll-content"><button class="mdc-ripple-upgraded mdc-ripple-upgraded--background-focused mdc-tab mdc-tab--min-width mdc-tab--active" aria-selected="true" tabindex="0">

<div class="mdc-tab__content"><span class="mdc-tab__text-label"><span>Java</span> <span class="shadow-text lang-badge java">Java</span></span></div>

<span class="mdc-tab-indicator mdc-tab-indicator--active"><span aria-hidden="true" class="mdc-tab-indicator__content mdc-tab-indicator__content--underline"></span></span></button></div>

</div>

</div>

</nav>

</div>

<div class="mt-2">

<div class="AnswerBody">

    public void reverse(Node head) {
        Node curr = head, prev = null;

        while (head.next != null) {
            head = head.next; // move the head to next node
            curr.next = prev; // break the link to the next node and assign it to previous
            prev = curr;      // we are done with previous, move it to next node
            curr = head;      // current moves along with head
        }

        head.next = prev;     //for last node
    }

</div>

</div>

</div>

<div class="row my-2">

<div><span>_Source:_ <span>[stackoverflow.com](https://stackoverflow.com/questions/1801549/how-to-reverse-a-singly-linked-list-using-only-two-pointers "How to reverse a singly Linked List using only two pointers? Interview Questions Source To Answer")</span></span>   </div>

</div>

</div>

</div>

</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 10\. What is complexity of push and pop for a Stack implemented using a LinkedList?

</div>

<div>

### Answer:

<div class="answer">

<div>

<div>

<div class="AnswerBody">

`_O_(_1_)`. Note, you don't have to insert at the end of the list. If you insert at the front of a (singly-linked) list, they are both `O(1)`.

Stack contains 1,2,3:

    [1]->[2]->[3]

Push 5:

    [5]->[1]->[2]->[3]

Pop:

    [1]->[2]->[3] // returning 5

</div>

</div>

<div class="row my-2">

<div><span>_Source:_ <span>[stackoverflow.com](https://stackoverflow.com/questions/6537150/time-complexity-of-a-stack-adt-implemented-using-a-linked-list#:~:text=For%20a%20doubly%20linked%20list,operations%20of%20enqueue%20and%20dequeue. "What is complexity of `push` and `pop` for a Stack implemented using a LinkedList? Interview Questions Source To Answer")</span></span>   </div>

</div>

</div>

</div>

</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 11\. Detect if a List is Cyclic using Hash Table

</div>

<div>

### Answer:

<div class="answer">

<div>

<div>

<div class="AnswerBody">

To detect if a list is cyclic, we can check whether a node had been visited before. A natural way is to use a hash table.

**Algorithm**

We go through each node one by one and record each node's reference (or memory address) in a hash table. If the current node is `null`, we have reached the end of the list and it must not be cyclic. If current node’s reference is in the hash table, then return true.

</div>

</div>

<div>

<div class="mb-2 mt-2"><span class="h5">Complexity Analysis</span></div>

<div class="hide-small">

<div class="row no-gutters my-2 align-items-end">

<div class="col font-weight-bold text-muted">Time:</div>

<div class="col disable text-center">

<div class="text-muted font-weight-bold justify-content-center">Constant</div>

<div class="complexity amazing first p-1 justify-content-center shadow-text">O(1)</div>

</div>

<div class="col disable text-center">

<div class="text-muted font-weight-bold justify-content-center">Dbl. Logarithmic</div>

<div class="complexity good p-1 justify-content-center shadow-text">O(log log n)</div>

</div>

<div class="col disable text-center">

<div class="text-muted font-weight-bold justify-content-center">Logarithmic</div>

<div class="complexity good p-1 justify-content-center shadow-text">O(log n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold  text-muted justify-content-center">Square Root</div>

<div class="complexity fair p-1 justify-content-center shadow-text ">O(√n)</div>

</div>

<div class="col text-center">

<div class="font-weight-bold  text-muted justify-content-center">Linear</div>

<div class="complexity fair p-1 justify-content-center shadow-text selected-complexity effect7">O(n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold text-muted justify-content-center">Linearithmic</div>

<div class="complexity bad p-1 justify-content-center shadow-text ">O(n log n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold  text-muted justify-content-center">Quadratic</div>

<div class="complexity terrible p-1 justify-content-center shadow-text ">_O_(_n_<sup>2</sup>)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold   text-muted justify-content-center">Exponential</div>

<div class="complexity terrible p-1 justify-content-center shadow-text ">_O_(_2_<sup>n</sup>)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold text-muted">Factorial</div>

<div class="complexity terrible last p-1 justify-content-center shadow-text ">O(n!)</div>

</div>

</div>

</div>

<div class="hide-small">

<div class="row no-gutters my-2 align-items-end">

<div class="col font-weight-bold text-muted">Space:</div>

<div class="col disable text-center">

<div class="text-muted font-weight-bold justify-content-center">Constant</div>

<div class="complexity amazing first p-1 justify-content-center shadow-text">O(1)</div>

</div>

<div class="col disable text-center">

<div class="text-muted font-weight-bold justify-content-center">Dbl. Logarithmic</div>

<div class="complexity good p-1 justify-content-center shadow-text">O(log log n)</div>

</div>

<div class="col disable text-center">

<div class="text-muted font-weight-bold justify-content-center">Logarithmic</div>

<div class="complexity good p-1 justify-content-center shadow-text">O(log n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold  text-muted justify-content-center">Square Root</div>

<div class="complexity fair p-1 justify-content-center shadow-text ">O(√n)</div>

</div>

<div class="col text-center">

<div class="font-weight-bold  text-muted justify-content-center">Linear</div>

<div class="complexity fair p-1 justify-content-center shadow-text selected-complexity effect7">O(n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold text-muted justify-content-center">Linearithmic</div>

<div class="complexity bad p-1 justify-content-center shadow-text ">O(n log n)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold   text-muted justify-content-center">Quadratic</div>

<div class="complexity terrible p-1 justify-content-center shadow-text ">_O_(_n_<sup>2</sup>)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold   text-muted justify-content-center">Exponential</div>

<div class="complexity terrible p-1 justify-content-center shadow-text ">_O_(_2_<sup>n</sup>)</div>

</div>

<div class="col disable text-center">

<div class="font-weight-bold text-muted">Factorial</div>

<div class="complexity terrible last p-1 justify-content-center shadow-text ">O(n!)</div>

</div>

</div>

</div>

<div class="hide-large">

**Time:** <mark>O(n)</mark>

**Space:** <mark>O(n)</mark>

</div>

<div class="mt-3">

<div>

<div class="AnswerBody">

*   Time complexity : `_O_(_n_)` . We visit each of the `n` elements in the list at most once. Adding a node to the hash table costs only `_O_(_1_)` time.
*   Space complexity: `_O_(_n_)` . The space depends on the number of elements added to the hash table, which contains at most `n` elements.

</div>

</div>

</div>

</div>

<div style="font-size: 14px;">

<div class="mb-3 mt-2"><span class="h5">Implementation</span></div>

<div>

<nav class="mdc-tab-bar">

<div class="mdc-tab-scroller">

<div class="mdc-tab-scroller__scroll-area mdc-tab-scroller__scroll-area--scroll" style="margin-bottom: 0px;">

<div class="mdc-tab-scroller__scroll-content"><button class="mdc-ripple-upgraded mdc-ripple-upgraded--background-focused mdc-tab mdc-tab--min-width mdc-tab--active" aria-selected="true" tabindex="0">

<div class="mdc-tab__content"><span class="mdc-tab__text-label"><span>Java</span> <span class="shadow-text lang-badge java">Java</span></span></div>

<span class="mdc-tab-indicator mdc-tab-indicator--active"><span aria-hidden="true" class="mdc-tab-indicator__content mdc-tab-indicator__content--underline"></span></span></button></div>

</div>

</div>

</nav>

</div>

<div class="mt-2">

<div class="AnswerBody">

    public boolean hasCycle(ListNode head) {
        Set<ListNode> nodesSeen = new HashSet<>();
        while (head != null) {
            if (nodesSeen.contains(head)) {
                return true;
            } else {
                nodesSeen.add(head);
            }
            head = head.next;
        }
        return false;
    }

</div>

</div>

</div>

<div class="row my-2">

<div><span>_Source:_ <span>[leetcode.com](https://leetcode.com/problems/linked-list-cycle/solution/ "Detect if a List is Cyclic using Hash Table Interview Questions Source To Answer")</span></span>   </div>

</div>

</div>

</div>

</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 12\. Convert a Singly Linked List to Circular Linked List

</div>

<div>

### Answer:

<div class="answer">

<div>

<div>

<div class="AnswerBody">

To convert a singly linked list to circular linked list, we will set next pointer of tail node to head pointer.

*   Create a copy of head pointer, let's say `temp`.
*   Using a loop, traverse linked list till tail node (last node) using temp pointer.
*   Now set the next pointer of tail node to head node. `temp\->next = head`

</div>

</div>

<div style="font-size: 14px;">

<div class="mb-3 mt-2"><span class="h5">Implementation</span></div>

<div>

<nav class="mdc-tab-bar">

<div class="mdc-tab-scroller">

<div class="mdc-tab-scroller__scroll-area mdc-tab-scroller__scroll-area--scroll" style="margin-bottom: 0px;">

<div class="mdc-tab-scroller__scroll-content"><button class="mdc-ripple-upgraded mdc-ripple-upgraded--background-focused mdc-tab mdc-tab--min-width mdc-tab--active" aria-selected="true" tabindex="0">

<div class="mdc-tab__content"><span class="mdc-tab__text-label"><span>Python</span> <span class="shadow-text lang-badge py">PY</span></span></div>

<span class="mdc-tab-indicator mdc-tab-indicator--active"><span aria-hidden="true" class="mdc-tab-indicator__content mdc-tab-indicator__content--underline"></span></span></button></div>

</div>

</div>

</nav>

</div>

<div class="mt-2">

<div class="AnswerBody">

    def convertTocircular(head):
        # declare a node variable
        # start and assign head
        # node into start node.
        start = head

        # check that
        while head.next
        # not equal to null then head
        # points to next node.
        while(head.next is not None):
          head = head.next

        #
        if head.next points to null
        # then start assign to the
        # head.next node.
        head.next = start
        return start

</div>

</div>

</div>

<div class="row my-2">

<div><span>_Source:_ <span>[www.techcrashcourse.com](https://www.techcrashcourse.com/2016/06/program-convert-singly-linked-list-to-circular-linked-list.html "Convert a Singly Linked List to Circular Linked List Interview Questions Source To Answer")</span></span>   </div>

</div>

</div>

</div>

</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 14\. Convert a Single Linked List to a Double Linked List

</div>

<div>

### Answer:

<div class="answer">

<div>

<div>

<div class="AnswerBody">

A doubly linked list is simply a linked list where every element has both next and prev mebers, pointing at the elements before and after it, not just the one after it in a single linked list.

so to convert your list to a doubly linked list, just change your node to be:

    private class Node
    {
        Picture data;
        Node pNext;
        Node pPrev;
    };

and when iterating the list, on each new node add a reference to the previous node.

</div>

</div>

<div class="row my-2">

<div><span>_Source:_ <span>[stackoverflow.com](https://stackoverflow.com/questions/9542154/converting-a-single-linked-list-to-a-double-linked-list/9542187#9542187 "Convert a Single Linked List to a Double Linked List Interview Questions Source To Answer")</span></span>   </div>

</div>

</div>

</div>

</div>

</div>

<div data-v-5e9078c0="" class="unit">

<div>

## 🔹 15\. When to use a Linked List over an Array/Array List?

</div>

<div>👉🏼 Check [all 43 answers](https://devinterview.io/data/linkedLists-interview-questions)</div>

</div>

Thanks 🙌 for reading and good luck on your next tech interview!  
Explore 3800+ dev interview question here 👉 [Devinterview.io](https://devinterview.io/)</div>
