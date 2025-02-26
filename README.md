# Student Tracker Application

This is a web-based application developed using Python's Flask framework. The application allows users to manage student records, including adding, editing, deleting, and viewing student information. Data is stored in a SQLite database for persistence.

## Features
- **Add Student**: Enter a student's name, age, and grade to add them to the student list.
- **Delete Student**: Select a student from the list and delete their record.
- **Edit Student**: Modify the details of an existing student.
- **View Students**: Display a list of all students with their details.
- **Search Students**: Search for students by name or grade.

## Code Details

### Key Components
- **SQLite Database**: Student records are stored in a SQLite database using SQLAlchemy for ORM (Object-Relational Mapping).
- **Flask Web Framework**: The user interface is built using Flask, with HTML templates for rendering pages.
- **CRUD Operations**: The app allows Create, Read, Update, and Delete operations on student records.

### Code Structure
```
student_tracker/
│── app.py         # Main application file
│── models.py      # Database model for Student entity
│── templates/     # HTML templates for rendering pages
│── static/        # Static files like CSS and JavaScript
│── requirements.txt # List of dependencies
│── README.md      # Project documentation
```

## Installation

### Requirements
- Python 3.x installed on your system.
- The following Python libraries are needed:
  - Flask
  - SQLAlchemy

### Setup Steps:
1. Clone or download this repository:
   ```bash
   git clone https://github.com/yourusername/student-tracker.git
   cd student-tracker
   ```
2. Install the required libraries:
   ```bash
   pip install Flask SQLAlchemy
   ```
3. Run the application:
   ```bash
   python app.py
   ```

## Database Structure

The student records are saved in a SQLite database with the following structure:

| ID | Name       | Age | Grade |
|----|-----------|-----|-------|
| 1  | John Doe  | 20  | A     |
| 2  | Jane Smith| 22  | B     |

- **ID**: Unique identifier for each student.
- **Name**: The name of the student.
- **Age**: The age of the student.
- **Grade**: The grade of the student.

## Application Walkthrough

### 1. Adding a Student
- Enter the student's name, age, and grade in the provided input fields.
- Click the "Add Student" button to add the student to the list.

### 2. Deleting a Student
- Select a student from the list.
- Click the "Delete Student" button to remove the selected student.

### 3. Editing a Student
- Select a student from the list.
- Click the "Edit Student" button. The student details will populate the input fields.
- Modify the student details and click the "Confirm Edit" button to save changes.

### 4. Viewing Students
- All students are displayed in a table format on the main page.

### 5. Searching for Students
- Use the search bar to find students by name or grade.

## Future Scope
- Add user authentication to secure student records.
- Implement a feature to upload student photos.
- Improve the UI with more modern styling.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.
