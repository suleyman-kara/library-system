# Library System (C++)

A simple, console-based Library Management System written in C++. It features book and member management, borrowing functionality with limits depending on the member type, and a built-in logging system.

## Features

- **Member Management**: Add, delete, and search members (Admin, Civilian, Student).
- **Book Management**: Add, delete, and search books by Title, ISBN, or ID.
- **Borrowing System**: Borrow and return books. Different member types have different borrowing limits:
  - Admin: 15 books
  - Civilian: 10 books
  - Student: 5 books
- **Logging**: All actions are automatically logged to a `log.txt` file with timestamps and log levels.

## Requirements

- A C++ compiler that supports the **C++17** standard (required for structured bindings).

## Compilation and Execution

Since the project uses C++17 features (like decomposition declarations/structured bindings), you must compile it with the `-std=c++17` flag.

1. Open your terminal and navigate to the root directory of the project.
2. Compile the source code using `g++`:

```bash
g++ -std=c++17 src/main.cpp -o main
```

3. Run the compiled executable:

```bash
./main
```

## Project Structure

- `src/main.cpp`: Contains the core logic for the library, entities (`Book`, `Member`), and the `IDGenerator` & `Logger` utility classes.
- `log.txt`: Generated automatically upon running the program to keep track of library events. 
