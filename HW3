# Exercise:

class Student:
    def __init__(self, name, student_id, gpa):
        self.__name = name
        self.__student_id = student_id
        self.__gpa = gpa
        self.__attendance = 0

    def mark_attendance(self):
        self.__attendance += 1

    def get_attendance(self):
        return self.__attendance

    def display_info(self):
        print(f"Name: {self.__name}, ID: {self.__student_id}, GPA: {self.__gpa}, Attendance: {self.__attendance}")

    def get_id(self):
        return self.__student_id


class Course:
    def __init__(self, course_name):
        self.course_name = course_name
        self.students = []

    def add_student(self, student):
        self.students.append(student)

    def remove_student(self, student_id):
        self.students = [s for s in self.students if s.get_id() != student_id]

    def list_students(self):
        print(f"Students enrolled in {self.course_name}:")
        for student in self.students:
            student.display_info()


# Sample usage
student1 = Student("Alice", "S12345", 3.8)
student2 = Student("Bob", "S67890", 3.5)

course = Course("Computer Science")
course.add_student(student1)
course.add_student(student2)

course.list_students()

student1.mark_attendance()
print("Attendance for Alice:", student1.get_attendance())
