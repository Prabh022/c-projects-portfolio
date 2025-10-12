# 🔧 Water Heater Management System (C)

A modular command-line management system for handling water heater inventory, installation scheduling, and staging operations. Built in C to simulate a small-scale business workflow with multiple user roles and secure login access.

---

## 🚀 Features

- Add and manage water heater inventory
- View and restock inventory with low-stock alerts
- Schedule installation appointments
- Stage tanks for installation
- Role-based access (Admin and Technician)
- Login system with authentication and access control
- Persistent storage using text files for all data

---

## 🧰 Technologies Used

- C (C99)
- File I/O (`fopen`, `fprintf`, `fscanf`, `fread`, `fwrite`)
- Structs, arrays, and string manipulation
- Modular architecture with multiple `.c` and `.h` files
- CLI-based menu navigation

---

## 📁 File Structure

water-heater-management/
├── main.c              # Entry point and user menu
├── inventory.c         # Add, view, and restock water heaters
├── inventory.h
├── installation.c      # Schedule and display installations
├── installation.h
├── staging.c           # Handle staging tanks for jobs
├── staging.h
├── users.c             # Authentication and user access
├── users.h
├── inventory.txt       # Inventory data file
├── installation.txt    # Installation records
├── staging.txt         # Staged tank records
├── users.txt           # User credentials and access levels
├── .gitignore          # Ignore build and IDE artifacts
└── README.md           # Project overview and usage

---

## 📦 How to Compile & Run

gcc main.c inventory.c installation.c staging.c users.c -o water_heater_mgmt  
./water_heater_mgmt

💡 All required `.txt` files will be created automatically if they do not exist.

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

# Optional: ignore data files if not versioning
inventory.txt
installation.txt
staging.txt
users.txt
