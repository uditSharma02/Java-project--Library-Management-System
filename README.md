# Library Management System

## Overview
A console-based Library Management System built in Java that allows adding, removing, searching, borrowing, and returning books. Data is persisted between sessions using file serialization.

## Real-World Problem / Need
Many small libraries and schools still manage books manually using registers. This leads to:
- Difficulty in finding books quickly
- No proper record of who borrowed what
- Books getting lost or misplaced
- Time-consuming stock verification

This project solves these issues by providing a simple digital solution.

## Objectives & Expected Outcomes
- Create a menu-driven application for library operations
- Apply core Java OOP concepts
- Implement data persistence
- Demonstrate clean, modular code design
- Provide a working, testable system

## Java Concepts Applied
- Classes and Objects
- Encapsulation (private fields + getters/setters)
- ArrayList and Collections
- Exception Handling
- File I/O (Serialization with ObjectOutputStream/ObjectInputStream)
- Method Overriding (toString())
- Control Structures and Loops

## Structured Development Process

### 1. Problem Definition
Inefficient manual management of library books (adding, searching, tracking availability).

### 2. Requirement Analysis
**Functional Requirements:**
- Add new book
- Remove book by ISBN
- Search book by ISBN and Title
- Borrow and return books
- Display all books
- Save data permanently

**Non-Functional Requirements:**
- Console-based interface
- Fast search operations
- Data should persist after program closes

### 3. Top-Down Design / Modularization
- **Book.java** → Entity class (data model)
- **Library.java** → Core logic and file handling
- **Main.java** → User interface and menu

### 4. Algorithm Development
- Linear search for ISBN and partial title match
- Serialization for saving/loading entire book list
- Availability flag toggle for borrow/return

### 5. Implementation
Three clean, well-commented classes with proper separation of concerns.

### 6. Testing & Refinement
Tested with:
- Adding multiple books
- Searching valid/invalid titles and ISBNs
- Borrowing and returning (including double-borrow prevention)
- Program restart → data still exists
- Error handling for file operations

## How to Run
1. Compile all files:
   ```bash
   javac *.java