# 📇 Contact Book (C)

A simple command-line contact management system built in C. This program lets users add, view, and search contacts stored in a text file for persistent storage. Designed to practice file handling, string operations, and modular programming.

---

## 🚀 Features

- Add new contacts with name, phone number, and email
- View all saved contacts
- Search contacts by name
- Persistent storage using a `.txt` file
- Menu-driven CLI interface

---

## 🧰 Technologies Used

- C (C99)
- File I/O (`fopen`, `fprintf`, `fscanf`)
- Structs and string manipulation (`strcpy`, `strcmp`)
- Modular design with header and implementation files

---

## 📁 File Structure

contact-book/
├── main.c              # CLI menu and control flow
├── contact.c           # Core logic: add, view, search
├── contact.h           # Function declarations and struct definitions
├── contacts.txt        # Persistent text-based storage
├── .gitignore          # Ignore build/IDE artifacts
└── README.md           # Project overview and usage

---

## 📦 How to Compile & Run

gcc main.c contact.c -o contact_book
./contact_book

💡 `contacts.txt` will be created automatically if it doesn’t exist.

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

# Optional: ignore contact data if not versioning
contacts.txt
