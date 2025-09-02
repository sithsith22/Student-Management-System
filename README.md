#### 1.Users

* UserID (PK)
* Username
* PasswordHash
* Role (Admin/Teacher)
#### 2.Students
* StudentID (PK)
* FirstName
* LastName
* Gender
* DateOfBirth
* Email (optional)
* Phone
* Address
* EnrollmentDate
* UserID (FK → Users)
#### 3.Courses
* CourseID (PK)
* CourseName
* Description (optional)
* Credits
#### 4.Enrollments
* EnrollmentID (PK)
* StudentID (FK → Students)
* CourseID (FK → Courses)
#### 5.Exams
* ExamID (PK)
* CourseID (FK → Courses)
* ExamName
* ExamDate
#### 6.ExamResults
* ResultID (PK)
* ExamID (FK → Exams)
* StudentID (FK → Students)
* Score
#### 7\. Feedback
* FeedbackID (PK)
* StudentID (FK → Students)
* Message
* DateSubmitted
* Status (Pending / Resolved)
#### 8.Payments (optional)
* PaymentID (PK)
* StudentID (FK → Students)
* Amount
* Date

Status

