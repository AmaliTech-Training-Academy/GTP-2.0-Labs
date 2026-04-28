# Student Grade Management System (Java OOP)

## Project Objectives
By completing this project, you will demonstrate the ability to:
* **Apply OOP principles** (Encapsulation, Inheritance, Polymorphism, Abstraction) to design real-world software solutions.
* **Create well-structured applications** integrating primitive types, control structures, and custom objects.
* **Analyze class relationships** to choose between inheritance, composition, abstract classes, and interfaces.
* **Evaluate code quality** using naming conventions and OOP best practices.

---

## 🏗 System Architecture

### Class Hierarchy & OOP Implementation
The system is built on **9 core classes** and **1 interface**:

1. **Student Hierarchy (Abstraction & Inheritance):**
    * `Student` (Abstract Class): Base for all students.
    * `RegularStudent` (Concrete): Passing grade 50%.
    * `HonorsStudent` (Concrete): Passing grade 60% + Honors eligibility.
2. **Subject Hierarchy:**
    * `Subject` (Abstract Class): Base for academic subjects.
    * `CoreSubject` (Concrete): Mandatory (Math, Science, etc.).
    * `ElectiveSubject` (Concrete): Optional (Art, Music, etc.).
3. **Logic & Management (Composition):**
    * `Gradable` (Interface): Defines grade recording and validation.
    * `Grade`: Represents a single grade record.
    * `StudentManager`: Manages an array of Students.
    * `GradeManager`: Manages an array of Grade records.
    * `Main`: The entry point and console menu controller.

---

## 🚀 Features & User Stories

### US-1: View Students
**As a teacher, I want to view all students so I can monitor performance.**
* Display ID, Name, Type, Average Grade, and Status.
* Shows Honors eligibility for qualified Honors students.
* Displays class-wide metrics (Total students, Class Average).

### US-2: Add Student
**As a teacher, I want to register new students.**
* Supports **Regular** and **Honors** types.
* Auto-generates unique Student IDs (e.g., `STU001`).
* Captures Name, Age, Email, and Phone.

### US-3: Record Grade
**As a teacher, I want to record grades for specific subjects.**
* Validates Student ID existence.
* Supports Core vs. Elective subject selection.
* **Validation:** Grades must be between 0 and 100.
* Auto-generates unique Grade IDs (e.g., `GRD001`).

### US-4: View Grade Report
**As a teacher, I want to see a detailed performance report for a specific student.**
* Lists full grade history.
* Calculates sub-averages for Core and Elective subjects.
* Summarizes passing status and performance alerts.

### US-5: Menu Navigation
**As a user, I want a simple console interface to navigate features.**
* Validates menu choices.
* Loops until "Exit" is selected.

---

## 💻 Console Examples

### Main Menu
```text
╔════════════════════════════════════════════╗
║    STUDENT GRADE MANAGEMENT - MAIN MENU    ║
╚════════════════════════════════════════════╝
1. Add Student
2. View Students
3. Record Grade
4. View Grade Report
5. Exit
