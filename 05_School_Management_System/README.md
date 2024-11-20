# School Management System

This is a Python-based **School Management System** project that allows you to manage students, courses, and teachers efficiently. The system allows for adding and managing courses, teachers, and students, and linking them to specific courses with relevant details such as grades and enrolled courses. It follows Object-Oriented Programming (OOP) principles for better structure and maintainability.

## Features

- **Student Management**: Allows adding and viewing student details, enrolled courses, and grades.
- **Teacher Management**: Manage teacher details and assign them to courses.
- **Course Management**: Create and manage courses, enroll students, and assign teachers to courses.
- **Dynamic Updates**: System updates student courses and grades dynamically.

## Classes in the Project

### 1. **Student**
   - **Attributes**:
     - `student_id`: Unique ID for each student.
     - `name`: Name of the student.
     - `enrolled_courses`: List of courses the student is enrolled in.
     - `grades`: A dictionary containing subjects and corresponding grades.
   - **Methods**:
     - `__str__`: Provides a string representation of the student's details.
   
### 2. **Teacher**
   - **Attributes**:
     - `teacher_id`: Unique ID for each teacher.
     - `name`: Name of the teacher.
     - `courses`: List of courses the teacher is teaching.
   - **Methods**:
     - `assign_course`: Assign a course to the teacher.
     - `__str__`: Provides a string representation of the teacher's details.

### 3. **Course**
   - **Attributes**:
     - `course_id`: Unique ID for each course.
     - `name`: Name of the course.
     - `students`: List of students enrolled in the course.
     - `teachers`: List of teachers teaching the course.
   - **Methods**:
     - `add_student`: Adds a student to the course.
     - `assign_teacher`: Assigns a teacher to the course.
     - `__str__`: Provides a string representation of the course's details.

### 4. **School**
   - **Attributes**:
     - `name`: Name of the school.
     - `courses`: List of courses available in the school.
     - `teachers`: List of teachers employed by the school.
     - `students`: List of students enrolled in the school.
   - **Methods**:
     - `add_course`: Adds a course to the school.
     - `add_teacher`: Adds a teacher to the school.
     - `add_student`: Adds a student to the school.

## Installation

To install and run this project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/YourUsername/School-Management-System.git
   ```

2. Navigate to the project directory:
   ```bash
   cd School-Management-System
   ```

3. Run the script:
   ```bash
   python main.py
   ```

## Usage

- Once the system is up and running, you can create instances of the **Student**, **Teacher**, **Course**, and **School** classes.
- The `__str__` method of each class allows you to print the details in a human-readable format.
- You can assign courses to students, add grades, assign teachers to courses, and manage all details dynamically.

## Example

Here is an example of how to use the classes:

```python
# Creating instances
student1 = Student("Abdullah", ["Python", "Java"], {"Python": "A", "Java": "B+"})
teacher1 = Teacher(1, "John Doe")
course1 = Course(101, "Python")
school = School("XYZ School")

# Assign courses to student and teacher
student1.enrolled_courses.append("Python")
teacher1.assign_course("Python")
course1.add_student("Abdullah")
course1.assign_teacher("John Doe")

# Add to school
school.add_student(student1)
school.add_teacher(teacher1)
school.add_course(course1)

# Print details
print(student1)
print(teacher1)
print(course1)
```

**Output:**

```plaintext
Student Name: Abdullah
Courses: Python, Java
Grades: Python: A, Java: B+
Teacher ID: 1
Name: John Doe
Courses: ['Python']
Course ID: 101
Name: Python
Students: ['Abdullah']
Teachers: ['John Doe']
```

## Contributing

If you want to contribute to this project, you are welcome to submit a pull request or open an issue. Please follow the standard guidelines for contributing to open-source projects.

## License

This project is open-source and available under the [MIT License](LICENSE).
```

### Explanation of Sections:

1. **Project Overview**: Describes what the project is and what it does.
2. **Features**: Lists the key functionalities of the system.
3. **Classes**: Detailed explanation of each class (Student, Teacher, Course, School) and their attributes and methods.
4. **Installation**: Instructions for setting up and running the project.
5. **Usage**: How to interact with the system using examples.
6. **Contributing**: Encourages others to contribute and provides a guideline for contribution.
7. **License**: States the license under which the project is shared (MIT License in this case).

