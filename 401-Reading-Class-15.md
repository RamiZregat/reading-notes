# Trees

## Introduction  
In this Note I.m going to discuss some topics. **Binary Trees**, **Binary Search Tree**s, and **K:ary Trees**, and to start we must introduce some common terminology first:  
### Common Terminology  
* Node :  
  > A Tree node is a component which may contain it’s own values, and references to other nodes
* Root   
  > The root is the node at the beginning of the tree
* K :  
  > A number that specifies the maximum number of children any node may have in a k:ary tree. In a binary tree, k = 2.
* Left :  
  > A reference to one child node, in a binary tree
* Right :  
  > A reference to the other child node, in a binary tree
* Edge :  
  > The edge in a tree is the link between a parent and child node
* Leaf :  
  > A leaf is a node that does not have any children
* Height :  
  > The height of a tree is the number of edges from the root to the furthest leaf.  
- [Top](#trees)
---
## Traversals  
Traversing a tree allows us to search for a node, and interact with trees values as we want.  
There are two categories of traversals when it comes to trees:
- Depth First
- Breadth First  
### Depth First  
In this method we traverse the tree according to its height, and for that we have three methods of traversing:  
  1. Pre-order : `root >> left >> right`
  1. In-order : `left >> root >> right`
  1. Post-order : `left >> right >> root`  
 
- The most common way to traverse through a tree is to use recursion. With these traversals, we rely on the call stack to navigate back up the tree when we have reached the end of a sub-path.

### Breadth First  
To traverse the tree in this method we iterate over the tree according to its levels. Each level is traversed in the order of `root >> left >> right`

Breadth first traversal uses a queue (instead of the call stack via recursion) to traverse the width/breadth of the tree. Let’s break down the process.  

## Binary Tree Vs K-ary Trees  
A **Binary Tree**, hence the name, each node can only have two child nodes. In **K-ary Trees**, each node can have a maximum of `K` number of children.  

We use **Breadth First** to traverse **K-ary Trees**, so we will be traversing as follow `root >> left >> as K nu,ber of child nodes in the middle >> right`. 

## Adding a node 
Because there are no structural rules for where nodes are “supposed to go” in a binary tree, it really doesn’t matter where a new node gets placed.  
If we want to fill the tree from top to bottom, then we can use **Breadth First** method.  
In the event you would like to have a node placed in a specific location, you need to reference both the new node to create, and the parent node upon which the child is attached to.  
### Big O  
The Big O time complexity for inserting a new node is `O(n)`, while the big O space complexity for a node insertion using breadth first insertion will be `O(w)`, where `w` is the largest width of the tree.

## Binary Search Trees  
A Binary Search Tree (BST) is a type of tree that does have some structure attached to it. In this type of trees, the right node value must be greater from the root node value, which in return is greater from the left node value, or as follow `right > root > left`.

### Searching a BST  
Searching a node in **BST** is easy. Just traverse the root first, if the value is greater, then traverse left. Ig it's smaller, then traverse right.

### Big O  
The Big O time complexity of a Binary Search Tree’s insertion and search operations is `O(h)`, where `h` represent the height of the tree.  
The Big O space complexity of a BST search would be `O(1)`. During a search, we are not allocating any additional space.  