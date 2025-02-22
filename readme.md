# Student Report Card Management System

A C++ console application for managing student academic records and generating report cards. This system allows teachers and administrators to maintain student records, including personal information and academic performance data.

## Features

- Create and manage student records with the following information:
  - Roll number
  - Student name
  - Subject marks (Physics, Chemistry, Mathematics, English, Computer Science)
  - Automatically calculated percentage and grades

- Complete CRUD operations:
  - Create new student records
  - Read/display individual and all student records
  - Update existing student records
  - Delete student records

- Additional functionalities:
  - Display class result in tabular format
  - Generate individual student report cards
  - Automatic grade calculation based on percentage
  - Data persistence using binary file storage

## Technical Details

- Language: C++
- File Handling: Binary file operations using fstream
- Data Storage: Records stored in 'student.dat' file
- Grade Calculation:
  - A: >= 60%
  - B: >= 50%
  - C: >= 33%
  - F: < 33%

## Menu Structure

1. Main Menu
   - Result Menu
   - Entry/Edit Menu
   - Exit

2. Result Menu
   - Class Result
   - Student Report Card
   - Back to Main Menu

3. Entry/Edit Menu
   - Create Student Record
   - Display All Students Records
   - Search Student Record
   - Modify Student Record
   - Delete Student Record
   - Back to Main Menu

## How to Use

1. Compile the program using a C++ compiler:
   ```bash
   g++ student-report-card-project.cpp -o student_management
   ```

2. Run the executable:
   ```bash
   ./student_management
   ```

3. Navigate through the menus using the number keys (1-6) as prompted.

## File Structure

The program uses a binary file (`student.dat`) to store student records. Each record contains:
- Roll number (integer)
- Name (character array)
- Marks in five subjects (integers)
- Percentage (double)
- Grade (character)

## Function Descriptions

- `write_student()`: Creates a new student record
- `display_all()`: Shows all stored student records
- `display_sp(int)`: Displays specific student record by roll number
- `modify_student(int)`: Updates existing student record
- `delete_student(int)`: Removes student record from file
- `class_result()`: Displays all students' results in tabular format
- `calculate()`: Computes percentage and grade based on marks

## Author

- Made by: Aman Kumar
- College: IIIT Bhagalpur

## Notes

- All marks should be entered out of 100
- The system automatically calculates percentage and assigns grades
- Data is persistently stored in binary format
- The program uses proper error handling for file operations
- Clean interface with clear menu options for easy navigation
