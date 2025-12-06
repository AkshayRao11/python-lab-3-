# 📚 Library Management System

# Project Overview

The **Library Management System** is a robust, CLI-based Python application designed to manage book inventories efficiently. It demonstrates core software engineering principles including Object-Oriented Programming (OOP), file persistence with JSON, modular architecture, and exception handling.

This system allows librarians to manage their catalog, issue/return books, and persist data across sessions, ensuring no data is lost when the program closes.

# ✨ Features

- 📖 **Book Management**: Add new books with details like Title, Author, and ISBN.

- 🔄 **Circulation System**: Issue books to members and accept returns, updating status in real-time.

- 💾 **Data Persistence**: Automatically saves and loads the inventory using a JSON database (library.json), ensuring data integrity.

- 🔍 **Search Functionality**:

  - Search for books by Title (case-insensitive partial match).
  - Find specific books by ISBN.

- 🛡️ **Robust Error Handling**: graceful handling of missing files, corrupted data, and invalid user inputs.

- 📝 **Logging**: Tracks important events and errors in a library.log file for debugging and auditing.

- ✅ **Modular Design**: Organized into separate modules for logic (library_manager) and interface (cli).

# 📂 Project Structure

```
LibraryProject/
├── library_manager/ # Core Logic Package
│ ├── **init**.py
│ ├── book.py # Book Class & Attributes
│ └── inventory.py # Inventory Management & JSON I/O
├── cli/ # User Interface Package
│ └── main.py # Main Entry Point
├── tests/ # Unit Tests
│ └── test.py
├── library.json # Database (Auto-generated)
├── library.log # Log File (Auto-generated)
├── requirements.txt # Dependencies
└── README.md # Project Documentation
```

# 🚀 Getting Started

**Prerequisites**

- Python 3.x installed on your system.

**Installation**

1. Clone or download this repository.

2. Navigate to the project directory:

```
cd LibraryProject
```

3. (Optional) Install test dependencies:

```
pip install -r requirements.txt
```

# 💻 Usage

To start the application, run the `main.py` script from the project root:

```
python cli/main.py
```

**Using the Menu:**

1. **Add Book**: Enter the book details. Duplicate ISBNs are prevented.

2. **Issue Book**: Mark a book as "issued" using its ISBN.

3. **Return Book**: Mark a book as "available" using its ISBN.

4. **Search**: Find books by title keywords.

5. **View All**: Display the entire catalog.

6. **Exit**: Close the program (data is saved automatically).

# 🧪 Running Tests (Bonus)

This project includes unit tests to verify the logic of the Book class. To run the tests:

```
python -m unittest tests/test.py
```

# 📝 Author

Name: Akshay Kumar

Date: 29/11/25
