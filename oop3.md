## Lab Exercise: Course and Instructor Classes

Create a Python program containing two classes: `Course` and `Instructor`.

### 1. Course class

Create a class named `Course` with the following attributes:

* Course name
* Course code
* Number of students
* Instructor

Add a method named `display_course()` to display all the course information.

### 2. Instructor class

Create a class named `Instructor` with the following attributes:

* Instructor ID
* Instructor name

Add a method named `display_instructor()` to display the instructor’s information.

### 3. Assign an instructor

Each course must have one instructor.

Create a method named `assign_instructor()` in the `Course` class. The method receives an `Instructor` object and assigns it to the course.

### 4. Test your program

Create:

* Two instructor objects
* Two course objects
* Assign one instructor to each course
* Display the information for both courses

### Expected output

```text
Course Code: CPAN101
Course Name: Introduction to Python
Number of Students: 25
Instructor: Mary Smith

Course Code: CPAN202
Course Name: Data Structures
Number of Students: 30
Instructor: Ahmed Ali
```

### Submission

Submit one Python file named:

```text
StudentName_CourseLab.py
```

#---
# Lab: Course and Instructor Management System

## Objective

In this lab, you will create an object-oriented Python program that manages courses and instructors.

The system must follow a **one-to-one relationship**:

* Each course can be assigned to only one instructor.
* Each instructor can teach only one course.

## Part A: Create the `Course` Class

Create a class named `Course` with the following attributes:

* `course_code`
* `course_name`
* `instructor`

When a course is created, its instructor should initially be set to `None`.

Add a method named `display_course()` that displays:

* Course code
* Course name
* Assigned instructor’s name

If the course does not have an instructor, display:

```text
Instructor: Not assigned
```

## Part B: Create the `Instructor` Class

Create a class named `Instructor` with the following attributes:

* `instructor_id`
* `instructor_name`
* `course`

When an instructor is created, their course should initially be set to `None`.

Add a method named `display_instructor()` that displays:

* Instructor ID
* Instructor name
* Assigned course name

If the instructor does not have a course, display:

```text
Course: Not assigned
```

## Part C: Assign an Instructor to a Course

Create a method named `assign_instructor()` in the `Course` class.

The method must receive an `Instructor` object and create the relationship in both directions:

* The course stores the assigned instructor.
* The instructor stores the assigned course.

Before completing the assignment, the method must verify that:

1. The course does not already have an instructor.
2. The instructor does not already teach another course.
3. The provided object is an instance of the `Instructor` class.

If the assignment is successful, display:

```text
Mary Smith has been assigned to Introduction to Python.
```

If the course already has an instructor, display:

```text
Assignment failed: This course already has an instructor.
```

If the instructor already teaches another course, display:

```text
Assignment failed: This instructor already teaches another course.
```

## Part D: Test the Program

Create at least:

* Three `Course` objects
* Three `Instructor` objects

Perform the following tests:

1. Assign one instructor to one course.
2. Assign a second instructor to a second course.
3. Try to assign the first instructor to another course.
4. Try to assign another instructor to a course that already has an instructor.
5. Display the information for all courses.
6. Display the information for all instructors.

## Expected Output Example

```text
Mary Smith has been assigned to Introduction to Python.
Ahmed Ali has been assigned to Data Structures.

Assignment failed: This instructor already teaches another course.
Assignment failed: This course already has an instructor.

Course Code: CPAN101
Course Name: Introduction to Python
Instructor: Mary Smith

Instructor ID: 1001
Instructor Name: Mary Smith
Course: Introduction to Python
```

## Part E: Advanced Requirement

Add a method named `remove_instructor()` to the `Course` class.

This method must:

* Remove the instructor from the course.
* Remove the course from the instructor.
* Display an appropriate message if no instructor is assigned.

After removing an instructor, both objects must show that they are no longer assigned.

## Submission Requirements

Submit one Python file named:

```text
StudentName_CourseInstructorLab.py
```

Your file must include:

* The `Course` class
* The `Instructor` class
* All required methods
* At least three courses and three instructors
* Tests demonstrating successful and unsuccessful assignments
* Comments explaining the important parts of the program

## Suggested Marking Scheme

| Requirement                       |  Marks |
| --------------------------------- | -----: |
| `Course` class and attributes     |      2 |
| `Instructor` class and attributes |      2 |
| Display methods                   |      2 |
| Correct one-to-one assignment     |      3 |
| Validation and error messages     |      2 |
| Required test cases               |      2 |
| `remove_instructor()` method      |      2 |
| Code quality and comments         |      1 |
| **Total**                         | **16** |
