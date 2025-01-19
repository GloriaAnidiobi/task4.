# task4.

UML Class Diagram (Plain Text)

Class: Student
Attributes:

studentId (String)

name (String)


Methods:

enroll()

viewGrades()


Class: Teacher
Attributes:

teacherId (String)

subject (String)


Methods:

assignGrade()

viewSchedule()



---

JavaScript Implementation

// Student Class
class Student {
  constructor(studentId, name) {
    this.studentId = studentId;
    this.name = name;
  }

  enroll() {
    console.log(`Student ${this.name} (ID: ${this.studentId}) has been enrolled.`);
  }

  viewGrades() {
    console.log(`Displaying grades for student ${this.name}.`);
  }
}

// Teacher Class
class Teacher {
  constructor(teacherId, subject) {
    this.teacherId = teacherId;
    this.subject = subject;
  }

  assignGrade(studentName, grade) {
    console.log(`Teacher (ID: ${this.teacherId}) assigned grade ${grade} to ${studentName}.`);
  }

  viewSchedule() {
    console.log(`Displaying schedule for teacher (ID: ${this.teacherId}).`);
  }
}

// Example Usage
const student1 = new Student("S101", "Alice");
student1.enroll();
student1.viewGrades();

const teacher1 = new Teacher("T201", "Mathematics");
teacher1.viewSchedule();
teacher1.assignGrade("Alice", "A+");


---

Explanation of Classes

1. Student Class:

Attributes:

studentId: A unique identifier for each student.

name: The name of the student.


Methods:

enroll(): Logs a message indicating the student has been enrolled.

viewGrades(): Displays the grades of the student.




2. Teacher Class:

Attributes:

teacherId: A unique identifier for each teacher.

subject: The subject the teacher is teaching.


Methods:

assignGrade(): Allows the teacher to assign a grade to a student.

viewSchedule(): Displays the teacher's schedule.

