# 🎲 Data Structures Game – Linked List & Binary Search Tree

This project is a Java-based game n developed to practice and demonstrate core Data Structures concepts, specifically **Linked Lists** and **Binary Search Trees (BST)**.

---

## 📌 Project Overview

The application consists of two main components:

1. 🎮 Game System (Linked List based board navigation)
2. 📊 Scoreboard System (Binary Search Tree based ranking)

The project demonstrates how fundamental data structures can be used in a practical and interactive application.

---

# 🎮 Game Part

## 🧩 Game Mechanics

- The game starts from a **Main Menu**
- User must enter a valid username
- Two options:
  - Play
  - Scoreboard

### 🎲 Gameplay

- The board contains **30 cells**
- Player starts at the **ST (Start) cell**
- Player rolls a dice (1–6)
- Moves forward based on dice result

### 🟢 Cell Types

Cells may contain actions such as:
- `+10 points`
- `-5 points`
- `Big prize`
- `Move forward`
- `Move backward`
- Some cells have no effect

### 🏁 Levels

**Level 1**
- Only score increasing/decreasing cells

**Level 2**
- Includes special mover cells
- More advanced movement logic

When reaching the **FN (Finish) cell**:
- Player can stop or continue to Level 2
- Scores are written to a `.txt` file
- Game statistics are displayed

---

## 🔗 Linked List Implementation

The game board is implemented using a **custom doubly linked list**.

Each `Cell` node contains:

- `action`
- `next`
- `prev`
- `alt` (used for special movers in Level 2)
- `JButton`
- `JLabel`

Movement logic:
- Normal movement → `next` / `prev`
- Special movement → `alt`

This structure allows dynamic and flexible navigation across the board.

---

# 📊 Scoreboard Part

The scoreboard system demonstrates **Binary Search Tree (BST)** usage.

## ⚙️ How It Works

1. Reads `score.txt` file  
   Format:  
2. Filters scores by username

3. Creates `Player` objects

4. Inserts players into a **Binary Search Tree**
- Sorted by score
- Smaller scores → left
- Larger scores → right

---

## 🌳 Binary Search Tree Operations

- `insert()` → Adds node based on score comparison
- `traverseInOrder()` → Sorts scores ascending
- `findMin()` → Finds worst score
- `findMax()` → Finds best score

---

## 🔁 Linked List + BST Combination

After BST is created:

- `traverseInOrder()` is used
- Each Player object is inserted into a Linked List
- Linked List is used to display sorted results in the UI

This demonstrates:
- Tree traversal
- Data transformation
- Hybrid data structure usage

---

# 🛠 Technologies Used

- Java
- Java Swing (GUI)
- File I/O (.txt score storage)

---

# 🎯 Data Structures Concepts Practiced

- Doubly Linked List
- Binary Search Tree
- Tree Traversal (InOrder)
- Recursive algorithms
- File handling
- OOP principles

---

# 👨‍💻 Authors
Hakan Kocaman  
Ahmet Emin Uğurlu  
---
