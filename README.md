# Student-Management-having-MySQL
# 🎓 Student Management System

A Python-based Student Management System using **MySQL** as the backend database — built as a Class 12 project by **Aakash Deep Kumar**.

## 📋 Features

- Add new student records (Roll No., Name, Date of Birth, Attendance)
- Search students by:
  - Roll Number
  - Name
  - Birth Year
  - Attendance status (Present / Absent)
- Data is stored persistently in a MySQL database
- Simple console-based menu interface

## 🛠️ Tech Stack

- **Python 3**
- **MySQL** (via `mysql-connector-python`)

## 📁 Project Structure

```
├── mysql1.py       # Main application file
└── README.md
```

## ⚙️ Prerequisites

1. Python 3 installed
2. MySQL Server installed and running
3. Install the MySQL connector:
   ```bash
   pip install mysql-connector-python
   ```

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/ap6107308/student-management-system.git
   cd student-management-system
   ```

2. Open `mysql1.py` and update your MySQL credentials:
   ```python
   mydb = mysql.connector.connect(
       host="localhost",
       user="root",
       passwd="your_password"   # change this
   )
   ```

3. Run the program:
   ```bash
   python mysql1.py
   ```

4. The database `student_db1` and table `student_tb` will be created automatically on first run.

## 🗄️ Database Schema

**Database:** `student_db1`  
**Table:** `student_tb`

| Column | Type        | Description            |
|--------|-------------|------------------------|
| sroll  | VARCHAR(30) | Roll No. (Primary Key) |
| sname  | VARCHAR(30) | Student Name           |
| sdob   | VARCHAR(30) | Year of Birth          |
| satt   | VARCHAR(30) | Attendance (P / A)     |

## 📌 Menu Options

```
[1] Entry of new student
[2] Search student
    ├── [1] Search by Roll No.
    ├── [2] Search by Name
    ├── [3] Search by Birth Year
    ├── [4] Search Present students
    ├── [5] Search Absent students
    └── [6] Back to Main Menu
```
