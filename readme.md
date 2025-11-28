# 🎓 Student Record Management System
### Java Programming Lab | Semester 3 Capstone Project

![Java](https://img.shields.io/badge/Language-Java-orange) ![Status](https://img.shields.io/badge/Status-Completed-brightgreen) ![Semester](https://img.shields.io/badge/Semester-3-blue)

A comprehensive, persistent, and multithreaded command-line application designed to manage student records. This project serves as a consolidation of **Lab Assignments 1 through 5**, demonstrating mastery of Object-Oriented Programming, Java Collections, and File I/O.

---

## 🚀 Key Features

* **PERSISTENT STORAGE**: Automatically saves and loads student records to a local file (`students.txt`) so data is never lost.
* **MULTITHREADING**: Features a simulated "Loading..." animation using background threads to mimic real-world data processing delays.
* **SMART SORTING**: Sorts students by **Marks (Descending)** using custom `Comparator` logic.
* **ROBUST VALIDATION**: Prevents duplicate Roll Numbers and validates input (e.g., Marks must be 0-100).
* **ERROR HANDLING**: Implements custom exceptions (`StudentNotFoundException`) for safer execution.
* **MODULAR ARCHITECTURE**: Clean separation of concerns using `model`, `service`, and `util` packages.

---

## 📂 Project Structure

The project follows a strict **Modular Design** pattern as per Lab 2 & 5 guidelines:

```text
StudentManagementSystem/
├── src/
│   ├── main/
│   │   └── Main.java                 # Entry point (Menu System)
│   ├── model/
│   │   ├── Person.java               # Abstract Base Class
│   │   └── Student.java              # Concrete Data Class
│   ├── service/
│   │   ├── RecordActions.java        # Interface for CRUD Operations
│   │   └── StudentManager.java       # Business Logic & File I/O
│   └── util/
│       ├── Loader.java               # Multithreading Simulation
│       └── StudentNotFoundException.java  # Custom Exception
├── students.txt                      # Data storage file
└── README.md