# Library Management System

## Overview
The **Library Management System** is a Python-based project designed to efficiently manage books and members of a library. It allows the issuance and return of books, while enforcing distinct rules for different member types such as students and teachers. The system leverages Object-Oriented Programming (OOP) principles like encapsulation, inheritance, abstraction, and polymorphism.

## Features
- **Add and Manage Books:** Easily add books to the library inventory and keep track of their availability.
- **Member Management:** Supports different member types (e.g., Students, Teachers) with specific borrowing limits.
- **Issue and Return Books:** Allows members to issue and return books with real-time availability updates.
- **Polymorphic Behavior:** Different rules and limits for students and teachers.
- **Error Handling:** Ensures proper validations and exceptions for incorrect operations.

## Class Structure
### 1. `Library`
- Manages the collection of books.
- Handles issuing and returning books.
- Tracks the inventory of available books.

### 2. `Book`
- Represents individual book details like title, author, and availability status.

### 3. `Member`
- A base class for library members with shared attributes like name and borrowed books.
- Abstract method to define the maximum books a member can borrow.

### 4. `Student` (inherits from `Member`)
- Implements rules specific to students (e.g., borrowing limit).

### 5. `Teacher` (inherits from `Member`)
- Implements rules specific to teachers (e.g., higher borrowing limit).

## Prerequisites
- Python 3.7 or higher
