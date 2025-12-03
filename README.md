# Binary Search Tree (BST) – Java Implementation

This project contains a clean and simple implementation of a **Binary Search Tree (BST)** in Java. The tree supports the following operations:

- Add a node  
- Search for a value  
- Remove a node (0, 1, or 2 children)  
- Print elements using **in-order traversal**  
- Count the number of leaf nodes  

## 📁 Project Structure
```
src/
 ├── Main.java
 ├── Node.java
 └── BinaryTree.java
```

## 📌 Class Overview

### Node.java  
Represents a single node in the tree.  
- data → value stored in the node  
- left → left child  
- right → right child  

### BinaryTree.java  
Contains the complete BST logic.

#### addNode(int data)  
Adds a new node to the tree (no duplicates allowed).

#### searchNode(int data)  
Returns true if the value exists in the tree.

#### removeNode(int data)  
Removes a node using the 3 classic BST deletion cases:  
1. Leaf node  
2. One child  
3. Two children → replaced with the **in-order successor**

#### printInOrder()  
Prints tree values in sorted (ascending) order.

#### countLeaves()  
Counts the total number of leaf nodes.

## ▶️ Running the Program

1. Clone the repository:
```bash
git clone https://github.com/yourusername/yourrepo.git
```

2. Compile:
```bash
javac Main.java BinaryTree.java Node.java
```

3. Run:
```bash
java Main
```

## 📘 How the BST Works

- Left subtree → values **less** than the node  
- Right subtree → values **greater** than the node  
- In-order traversal prints values in **ascending order**  
- Search, insert, delete operations run in **O(log n)** time on a balanced tree  

## 📝 Example In-Order Output
```
4 10 16 32 36 48 64 66 72 87 114 128 150
```

## 🤝 Contributing

Pull requests and improvements are welcome. You may extend the project with AVL rotations, Red-Black Tree balancing, or visualization features.

## 📄 License

This project is licensed under the MIT License.
