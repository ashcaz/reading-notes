# Linked Lists

**LINKS**

- [Linked Lists](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/singly_linked_list.html)
- [What’s a Linked List, Anyway pt1](https://medium.com/basecs/whats-a-linked-list-anyway-part-1-d8b7e6508b9d)
- [What’s a Linked List, Anyway pt2](https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996)


## Code Fellows: Linked Lists

### What is a Linked List

A Linked List is a sequence of `Nodes` that are connected/linked to each other. The most defining feature of a Linked List is that each `Node` references the next `Node` in the link

There are two types of Linked List - **Singly** and **Doubly**.

**Terminology**

1. Singly - Singly refers to the number of references the node has. A Singly linked list means that there is only one reference, and the reference points to the Next node in a linked list.
2. Doubly - Doubly refers to there being two (double) references within the node. A Doubly linked list means that there is a reference to both the Next and Previous node.
3. Node - Nodes are the individual items/links that live in a linked list. Each node contains the data for each link.
Next - Each node contains a property called Next. This property contains the reference to the next node.
4. Head - The Head is a reference type of type Node to the first node in a linked list.
5. Current - The Current reference is a reference type of type Node that is currently being looked at. This node is traditionally used when traversing through a full linked list. When traversing, you typically reset the current to the head to guarantee you are starting from the beginning of the linked list.

### Traversal

When traversing a linked list, you are not able to use a `foreach` or `for` loop. We depend on the `Next` value in each node to guide us where the next reference is pointing. The `Next` property is exceptionally important because it will lead us where the next node is and allow us to extract the data appropriately.

The best way to approach a traversal is through the use of a while() loop. This allows us to continually check that the Next node in the list is not null. If we accidentally end up trying to traverse on a node that is null, a NullReferenceException gets thrown and our program will crash/end.

[Back to Homepage](https://ashcaz.github.io/reading-notes)

### Adding a Node