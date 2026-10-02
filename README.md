# Student Management System

A Python-based console application for managing student records using Object-Oriented Programming, exception handling, and file handling.

---

## What the Project Does

The **Student Management System** is a menu-driven Python application that allows users to manage student records.

Each student record contains:

- Roll Number
- Student Name
- Marks

The application allows users to:

1. Add Student
2. Display Students
3. Search Student
4. Update Student
5. Delete Student
6. Calculate Average Marks
7. Save Records
8. Exit

Student records are stored in a `students.txt` file so that existing records can be loaded when the program starts.

---

## How the Project Works

When the program starts, the `StudentManager` loads existing student records from the `students.txt` file using the `FileManager` class.

The user is then shown a menu with eight options.

![Add Student](https://github.com/Rollybuilds/Student_Management_System/blob/8a829e6499e324b8e27804fa68531108ba6c02d0/Enter%20Your%20choice.png)

### Add Student 

![Add Student](https://github.com/Rollybuilds/Student_Management_System/blob/8a829e6499e324b8e27804fa68531108ba6c02d0/Student%20Added.png)
The user enters:

- Roll Number
- Student Name
- Marks

The program validates the information before adding the student.

- Roll number cannot be empty.
- Duplicate roll numbers are not allowed.
- Name cannot be empty.
- Name cannot contain `|`.
- Marks must be between `0` and `100`.

### Display Students

Displays all student records currently stored in the system.

![Add Student](https://github.com/Rollybuilds/Student_Management_System/blob/f3fc64d60e4e79615b0f8a15db514c40b793e6a1/Records%20Displayed.png)

### Search Student

The user enters a roll number. The program searches for the student and displays the student's details if found.

![Add Student](https://github.com/Rollybuilds/Student_Management_System/blob/f3fc64d60e4e79615b0f8a15db514c40b793e6a1/Search%20Student.png)

### Update Student

The user can update:

- Student Name
- Marks

  ![Add Student](https://github.com/Rollybuilds/Student_Management_System/blob/f3fc64d60e4e79615b0f8a15db514c40b793e6a1/Update%20Student.png)

The new values are validated before updating the existing record.


### Delete Student

The user enters a roll number, and the matching student record is removed.

![Add Student](https://github.com/Rollybuilds/Student_Management_System/blob/f3fc64d60e4e79615b0f8a15db514c40b793e6a1/Delete%20Student.png)

### Calculate Average Marks

The program calculates and displays:

- Total number of students
- Average marks
![Add Student](https://github.com/Rollybuilds/Student_Management_System/blob/f3fc64d60e4e79615b0f8a15db514c40b793e6a1/Average%20Student.png)

### Save Records

All student records are saved to the `students.txt` file.

![Add Student](https://github.com/Rollybuilds/Student_Management_System/blob/f3fc64d60e4e79615b0f8a15db514c40b793e6a1/Record%20saved%20successfully.png)

### Exit

Before exiting, the program automatically saves all current student records.

![Add Student](https://github.com/Rollybuilds/Student_Management_System/blob/f3fc64d60e4e79615b0f8a15db514c40b793e6a1/Exit.png)

---

## How to Run the Project

### Google Colab

1. Open `Student_Management_System.ipynb` in Google Colab.
2. Upload the `students.txt` file using the **Files** section.
3. Run the Python code cells from top to bottom.
4. The Student Management System menu will appear.
5. Enter a number from `1` to `8`.
6. Follow the instructions displayed in the console.

## Classes Used

### 1. Person

`Person` is an abstract base class that stores the student name and defines the abstract `display_info()` method.

### 2. Student

`Student` inherits from `Person` and manages the student's roll number, name, and marks. It also provides getters, setters, validation, and student information display.

### 3. FileManager

`FileManager` handles saving and loading student records from the `students.txt` file and manages file-related errors.

### 4. StudentManager

`StudentManager` manages all student records and performs operations such as adding, displaying, searching, updating, deleting, calculating average marks, and saving records.

---
## Main Features Implemented

- Add new student records
- Display all student records
- Search students by roll number
- Update student information
- Delete student records
- Calculate average marks
- Prevent duplicate roll numbers
- Validate student names and roll numbers
- Validate marks between 0 and 100
- Handle invalid user input
- Handle invalid records in the text file
- Save student records to `students.txt`
- Load existing records when the program starts
- Automatically save records before exiting
- Menu-driven console interface
