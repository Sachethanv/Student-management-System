# Student Management System

## Introduction

A modern, user-friendly desktop application for managing student records efficiently. This Student Management System provides an intuitive graphical interface built with PyQt6, allowing educational institutions to seamlessly add, search, edit, and delete student information with a MySQL database backend.

## Features

- **Add Students**: Easily add new student records with name, course, and mobile number
- **Search Functionality**: Quick search capability to find students by name
- **Edit Records**: Update existing student information with a user-friendly interface
- **Delete Records**: Remove student records with confirmation dialogs
- **Database Integration**: Persistent storage using MySQL database
- **Modern GUI**: Clean and intuitive interface built with PyQt6
- **Table View**: Display all student records in an organized, sortable table
- **Menu System**: File and Help menus with About dialog

## Tech Stack

- **Python 3.x**: Core programming language
- **PyQt6**: GUI framework for desktop application
- **MySQL**: Database management system
- **mysql-connector-python**: MySQL database connector for Python

## Setup

### Prerequisites

- Python 3.x installed on your system
- MySQL Server installed and running
- pip (Python package manager)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/Sachethanv/Student-management-System.git
cd Student-management-System
```

2. Install required dependencies:
```bash
pip install PyQt6
pip install mysql-connector-python
```

3. Set up MySQL database:
- Create a MySQL database named `school`
- Create a table named `students` with columns: `id`, `name`, `course`, `mobile`
- Update the database credentials in `main.py` if needed

```sql
CREATE DATABASE school;
USE school;
CREATE TABLE students (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(255) NOT NULL,
    course VARCHAR(255) NOT NULL,
    mobile VARCHAR(20)
);
```

## Usage

1. Run the application:
```bash
python main.py
```

2. **Adding a Student**:
   - Click on the toolbar "Add" button or go to File → Add Student
   - Fill in the student's name, course, and mobile number
   - Click Submit

3. **Searching for Students**:
   - Click on the toolbar "Search" button or go to File → Search
   - Enter the student's name
   - Click Search to view results

4. **Editing Student Records**:
   - Select a student row in the table
   - Right-click and choose "Edit Record" or use the Edit menu
   - Update the information and click Update

5. **Deleting Student Records**:
   - Select a student row in the table
   - Right-click and choose "Delete Record" or use the Edit menu
   - Confirm the deletion

## License

This project is open source and available for educational purposes.

## Contact

**Developer**: Sachethanv

**GitHub**: [Sachethanv](https://github.com/Sachethanv)

**Repository**: [Student-management-System](https://github.com/Sachethanv/Student-management-System)

For issues, feature requests, or contributions, please open an issue on the GitHub repository.

---

*Built with ❤️ using Python and PyQt6*
