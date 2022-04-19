# What is Trees ?

***It is a data structure , non-linear data structure , because it does not store in a sequential manner. It is a hierarchical structure as elements in a Tree are arranged in multiple levels. In the Tree data structure, the topmost node is known as a root node. Each node contains some data, and data can be of any type.***

## Common Terminology

- **Node** : *A Tree node is a component which may contain its own values, and references to other nodes*

- **Root** : *The root is the node at the beginning of the tree*

- **K** : *A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2*

- **Left** : *A reference to one child node, in a binary tree*

- **Right** : *A reference to the other child node, in a binary tree*

- **Edge** : *The edge in a tree is the link between a parent and child node*

- **Leaf** : *A leaf is a node that does not have any children*

- **Height** : *The height of a tree is the number of edges from the root to the furthest leaf*


![IMG](https://debug.to/?qa=blob&qa_blobid=4157716542154707901)

## Traversals

***An important aspect of trees is how to traverse them. Traversing a tree allows us to search for a node, print out the contents of a tree, and much more! There are two categories of traversals when it comes to trees***:

- **Depth First**
- **Breadth First**

- ***Depth First*** :

***Depth first traversal is where we prioritize going through the depth (height) of the tree first. There are multiple ways to carry out depth first traversal, and each method changes the order in which we search/print the root. Here are three methods for depth first traversal***:

- **Pre-order** : *root >> left >> right*
- **In-order** : *left >> root >> right*
- **Post-order** : *left >> right >> root*

- ***Breadth First*** :

***Breadth first traversal iterates through the tree by going through each level of the tree node-by-node***

## Trees types :

***We will cover 3 types of Trees : ***

1. **Binary Trees** : ***A tree that every node in it has maximum 2 children , (K = 2)***

2. **Binary Search Trees** : ***A Binary Search Tree (BST) is a type of tree that does have some structure attached to it. In a BST, nodes are organized in a manner where all values that are smaller than the root are placed to the left, and all values that are larger than the root are placed to the right***

3. **K-ary Trees** : ***If Nodes are able have more than 2 child nodes, we call the tree that contains them a K-ary Tree. In this type of tree we use K to refer to the maximum number of children that each Node is able to have***

