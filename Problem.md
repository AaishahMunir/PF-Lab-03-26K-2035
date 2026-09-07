# Problem.md – Pseudocode

## 1. Display student information using different data types

START
DECLARE name AS string
DECLARE rollNumber AS integer
DECLARE gpa AS float
DECLARE grade AS character
INPUT name
INPUT rollNumber
INPUT gpa
INPUT grade

PRINT "Name: " name
PRINT "Roll Number: " rollNumber
PRINT "GPA: " gpa
PRINT "Grade: " grade

END

## 2. Read and display a character using getchar() and putchar()

START
DECLARE ch AS character

PRINT "Enter a character: "
ch = getchar()

PRINT "You entered: "
putchar(ch)

END


## 3. Display a floating-point value using different precision settings

START
DECLARE num AS float
num = 3.14159265

PRINT num WITH 2 decimal places
PRINT num WITH 4 decimal places
PRINT num WITH 6 decimal places

END
