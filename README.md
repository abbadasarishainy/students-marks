# students-marks
student marks 
Student Marks Management System – Python Project

print("========================================")
print("     STUDENT MARKS MANAGEMENT SYSTEM")
print("========================================")

# Student details
name = input("Enter Student Name: ")
roll_no = input("Enter Roll Number: ")

# Subject marks
python_marks = float(input("Enter Python Marks: "))
java_marks = float(input("Enter Java Marks: "))
c_marks = float(input("Enter C Marks: "))
maths_marks = float(input("Enter Maths Marks: "))
english_marks = float(input("Enter English Marks: "))

# Calculate total
total = python_marks + java_marks + c_marks + maths_marks + english_marks

# Calculate percentage
percentage = total / 5

# Calculate grade
if percentage >= 90:
    grade = "A+"
elif percentage >= 80:
    grade = "A"
elif percentage >= 70:
    grade = "B"
elif percentage >= 60:
    grade = "C"
elif percentage >= 50:
    grade = "D"
else:
    grade = "F"

# Check Pass or Fail
if (python_marks >= 35 and
    java_marks >= 35 and
    c_marks >= 35 and
    maths_marks >= 35 and
    english_marks >= 35):
    result = "PASS"
else:
    result = "FAIL"

# Display result
print("\n========================================")
print("             STUDENT RESULT")
print("========================================")

print("Student Name :", name)
print("Roll Number  :", roll_no)
print("Total Marks  :", total)
print("Percentage   :", percentage, "%")
print("Grade        :", grade)
print("Result       :", result)

print("========================================")

