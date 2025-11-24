**University Management System**
**Project Overview**
This University Management System is a Java-based console application that manages students, courses, enrollments, and grading.
It is designed to demonstrate key Java concepts such as:
•	OOP principles (Encapsulation, Inheritance, Polymorphism)
•	Java Collections Framework (List, Map, Stream API)
•	Java Date/Time API (LocalDate, LocalDateTime)
•	File I/O using NIO.2 for importing/exporting CSV files
•	Menu-driven CLI with loops, switch statements, and labeled jumps
 Features
•	Student Management: Add, list, update, and deactivate students
•	Course Management: Add, list, update, deactivate, and search courses by instructor, department, or semester
•	Enrollment & Grading: Enroll/unenroll students, record marks, compute grades & GPA, print transcripts
•	File Operations: Import/export students and courses from CSV files, create backups, and recursively compute directory sizes
________________________________________
 Tech Stack
•	Language: Java
•	JDK Version: Java 17 or later (tested on JDK 17 & JDK 21)
•	Build Tool: None (Plain Java – can compile with javac)
•	Dependencies: None (only standard Java libraries)
________________________________________
 How to Run
 Install JDK
Make sure Java JDK 17 or later is installed.
•	Check version:
java -version
Example output:
java version "17.0.10" 2024-01-16 LTS
If you don’t have JDK 17+, download it from:
👉 https://adoptium.net/ or Oracle JDK
________________________________________
 Clone or Download the Project
git clone https://github.com/your-username/university-management-java.git
cd university-management-java/src
If you downloaded a ZIP, unzip it and cd into the src folder.
________________________________________
 Compile the Project
Run the following inside the src folder (where the java_project package is located):
javac java_project/*.java
This compiles all .java files into .class files inside the same package.
________________________________________
 Run the Application
After successful compilation, run the MasterCLI main class:
java java_project.MasterCLI
________________________________________
 (Optional) Import CSV Files
To test File Operations, prepare CSV files like:
📄 students.csv
id,regNo,fullName,email,dateOfBirth
1,REG2025-001,John Doe,john@example.com,2001-05-14
2,REG2025-002,Jane Smith,jane@example.com,2002-03-22
 courses.csv
code,title,credits,instructor,semester,department
CS101,Intro to Programming,3,Dr. Allen,SPRING,Computer Science
MA201,Linear Algebra,4,Prof. Lee,FALL,Mathematics
In the CLI:
Main Menu -> File Operations -> Import Students/Courses
________________________________________
 Example Commands
•	List all students:
Main Menu -> Student Management -> List Students
•	Enroll a student:
Main Menu -> Enrollment & Grading -> Enroll Student
•	Generate transcript:
Main Menu -> Enrollment & Grading -> Print Transcript
________________________________________
 Project Structure
src/
└── java_project/
    ├── MasterCLI.java        # Main menu-driven CLI
    ├── Student.java           # Student entity
    ├── StudentManager.java    # Manage students
    ├── Course.java            # Course entity
    ├── CourseManager.java     # Manage courses
    ├── EnrollmentManager.java # Enrollment & grading logic
    ├── FileOperations.java    # CSV import/export utilities
    ├── Semester.java          # Enum for semesters
    └── GradeCalculator.java   # Utility for GPA & grade calculations
________________________________________
 Recommended JDK
JDK Version	Status
JDK 17	 Tested
JDK 21	Tested
JDK 11	May work (update switch expressions if needed)
________________________________________
 Tips
•	Always run commands inside the src folder.
•	Use CSV files with proper formatting to avoid parsing errors.
•	To clear compiled files:
rm java_project/*.class
