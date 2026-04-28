Student Grade Management System

Project Objectives

By completing this project, you will be able to:

Apply OOP principles (encapsulation, inheritance2, polym2orphism) to design Java classes and interfaces for real-world problems

Create well-structured applications integrating primitive data types, control structures, and custom objects

Analyze class relationships to choose between inheritance, composition, abstract classes, and interfaces

Evaluate code quality using proper encapsulation, naming conventions, and OOP best practices

Apply polymorphic behavior with method overriding to build flexible, extensible code

What You'll Build

A console application for managing student grades with these features:

Core Features

Add Student - Register new students in the system
View Students - Display all students with their details
Record Grade - Add grades for students in different subjects
View Grade Report - Display grade history for a student
Simple Menu - Navigate through options

Student Types

Regular Student - standard grading (passing grade: 50%)
Honors Student - higher standards (passing grade: 60%, eligible for honors recognition)

Subject Types

Core Subject - mandatory subjects (Mathematics, English, Science)
Elective Subject - optional subjects (Music, Art, Physical Education)

Console Output Examples

Screenshot 1: Main Menu

╔════════════════════════════════════════════╗
║   STUDENT GRADE MANAGEMENT - MAIN MENU     ║
╚════════════════════════════════════════════╝

1. Add Student
2. View Students
3. Record Grade
4. View Grade Report
5. Exit

Enter choice: _

Screenshot 2: View Students

Enter choice: 2

STUDENT LISTING
──────────────────────────────────────────────────────────────────────────
STU ID   | NAME              | TYPE         | AVG GRADE | STATUS
──────────────────────────────────────────────────────────────────────────
STU001   | Alice Johnson     | Regular      | 78.5%     | Passing
| Enrolled Subjects: 5 | Passing Grade: 50%
──────────────────────────────────────────────────────────────────────────
STU002   | Bob Smith         | Honors       | 85.2%     | Passing
| Enrolled Subjects: 6 | Passing Grade: 60% | Honors Eligible
──────────────────────────────────────────────────────────────────────────
STU003   | Carol Martinez    | Regular      | 45.0%     | Failing
| Enrolled Subjects: 4 | Passing Grade: 50%
──────────────────────────────────────────────────────────────────────────
STU004   | David Chen        | Honors       | 92.8%     | Passing
| Enrolled Subjects: 6 | Passing Grade: 60% | Honors Eligible
──────────────────────────────────────────────────────────────────────────
STU005   | Emma Wilson       | Regular      | 67.3%     | Passing
| Enrolled Subjects: 5 | Passing Grade: 50%
──────────────────────────────────────────────────────────────────────────

Total Students: 5
Average Class Grade: 73.8%

Press Enter to continue...

Screenshot 3: Add Student (Regular)
... (unchanged content continues exactly as you provided above)

User Stories
... (unchanged)

Minimum Requirements
... (unchanged)

Testing the Application

Test Scenario 1: View Students
Run application
Select option 2 (View Students)
Verify 5 students display with correct information
Check Regular students show 50% passing grade
Check Honors students show 60% passing grade and honors eligibility
Verify total students and average class grade calculations

Test Scenario 2: Add Regular Student
Select option 1 (Add Student)
Enter student details (name, age, email, phone)
Select Regular Student type
Verify unique student ID is generated (STU001, STU002, etc.)
Verify confirmation displays all details
Verify passing grade shows 50%

Test Scenario 3: Add Honors Student
Select option 1 (Add Student)
Enter student details
Select Honors Student type
Verify honors eligibility is shown
Verify passing grade shows 60%

Test Scenario 4: Record Grade (Core Subject)
Add at least one student first
Select option 3 (Record Grade)
Enter valid student ID
Select Core Subject
Choose a core subject (Mathematics, English, or Science)
Enter grade (75)
Verify grade ID is generated
Confirm grade

Test Scenario 5: Record Grade (Elective Subject)
Select option 3 (Record Grade)
Enter valid student ID
Select Elective Subject
Choose an elective (Music, Art, or Physical Education)
Enter grade (88)
Verify transaction succeeds

Test Scenario 6: Grade Validation
Select option 3 (Record Grade)
Enter student ID
Try to enter grade < 0
Verify system rejects it
Try to enter grade > 100
Verify system rejects it
Enter valid grade (0-100)
Verify system accepts it

Test Scenario 7: View Grade Report (Empty)
Add new student
Select option 4 (View Grade Report)
Enter new student ID
Verify "No grades recorded" message displays

Test Scenario 8: View Grade Report (With Records)
Record 3-5 grades for one student (mix of core and elective)
Select option 4 (View Grade Report)
Enter student ID
Verify all grades display correctly
Verify averages calculate correctly (core, elective, overall)
Verify passing status is correct

Test Scenario 9: Honors Eligibility Check
Add Honors student
Record grades averaging >= 85%
View student listing
Verify "Honors Eligible" appears
Record grades averaging < 85%
View student listing
Verify honors eligibility changes

Test Scenario 10: Unit Tests Execution
Run all JUnit tests: mvn test or IDE test runner
Verify all 25+ unit tests pass
Run integration tests
Verify all 10+ integration tests pass
Generate coverage report: mvn jacoco:report
Verify 85%+ coverage achieved
Check collections performance tests results
Check concurrency tests pass (no race conditions detected)
Review test execution time
Document any failed tests and reasons
