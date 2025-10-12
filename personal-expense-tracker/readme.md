# 💰 Personal Expense Tracker (C)

A modular command-line expense tracker built in C. This tool allows users to log, view, edit, and delete personal expenses, with persistent storage and summary reporting. Designed to practice file I/O, modular architecture, and real-world CLI workflows.

---

## 🚀 Features

- Add, view, edit, and delete expenses
- Generate summary reports (total, category-wise, etc.)
- Persistent storage using a `.dat` file
- Modular structure with reusable components
- Simple CLI interface for fast interaction

---

## 🧰 Technologies Used

- C (C99)
- File I/O (`fopen`, `fread`, `fwrite`)
- Structs and arrays
- Modular design (`main.c`, `expense.c`, `storage.c`, `report.c`)
- Header files for clean separation

---

## 📁 File Structure

personal-expense-tracker/
├── main.c              # CLI menu and control flow
├── expense.c           # Add, view, edit, delete logic
├── expense.h
├── storage.c           # File read/write operations
├── storage.h
├── report.c            # Summary report generation
├── expenses.dat        # Binary file for persistent storage
├── .gitignore          # Ignore build and IDE artifacts
└── README.md           # Project overview and usage

---

## 📦 How to Compile & Run

gcc main.c expense.c storage.c report.c -o expense_tracker
./expense_tracker

💡 expenses.dat will be created automatically if it doesn't exist.

---

## 🧹 .gitignore

# Build artifacts
*.o
*.out
*.exe

# IDE and OS junk
.vs/
.vscode/
*.ipch
*.log
.DS_Store
Thumbs.db

# Optional: ignore data file if not versioning
expenses.dat
