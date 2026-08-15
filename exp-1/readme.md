#WEEK-1 DBMSLAB
#students table creation
CREATE TABLE student (
    name VARCHAR2(50),
    student_number NUMBER,
    class VARCHAR2(20),
    major VARCHAR2(20)
);
![output](screenshots/output-week1/output-a.png)

#course table creation
CREATE TABLE course (
    course_name VARCHAR2(50),
    course_number VARCHAR2(10),
    credit_hours NUMBER,
    department VARCHAR2(30)
);
![output](screenshots/output-week1/output-b.png)

#section table creation
CREATE TABLE section (
    section_identifier NUMBER,
    course_number VARCHAR2(10),
    semester VARCHAR2(20),
    year NUMBER,
    instructor VARCHAR2(50)
);
![output](screenshots/output-week1/output-c.png)

#grade_report table creation
CREATE TABLE grade_report (
    student_number NUMBER,
    section_identifier NUMBER,
    grade VARCHAR2(1)
);
![output](screenshots/output-week1/output-d.png)

#ddescribing of tables
DESC student;
![output](screenshots/output-week1/desc-student.png)

DESC course;
![output](screenshots/output-week1/desc-course.png)

DESC section;
![output](screenshots/output-week1/desc-section.png)

DESC grade_report;
![output](screenshots/output-week1/desc-gradereport.png)

#insertion into student
INSERT INTO student VALUES ('Smith', 17, 1, 'CS');
INSERT INTO student VALUES ('Brown', 18, 2, 'CS');
![output](screenshots/output-week1/insert-student.png)

#insertion into course
INSERT INTO course VALUES ('Intro to Computer Science', 'CS1310', 4, 'CS');
INSERT INTO course VALUES ('Data Structures', 'CS3320', 4, 'CS');
INSERT INTO course VALUES ('Discrete Mathematics', 'MATH2410', 3, 'MATH');
INSERT INTO course VALUES ('Database Systems', 'CS3380', 3, 'CS');
![output](screenshots/output-week1/insert-course.png)

#insertion into section
INSERT INTO SECTION VALUES(85,'MATH2410','Fall',07,'King');
INSERT INTO SECTION VALUES(92,'CS1310','Fall',07,'Anderson');
INSERT INTO SECTION VALUES(102,'CS3320','Spring',08,'Knuth');
INSERT INTO SECTION VALUES(112,'MATH2410','Fall',08,'Chang');
INSERT INTO SECTION VALUES(119,'CS1310','Fall',08,'Anderson');
INSERT INTO SECTION VALUES(135,'CS3320','Fall',08,'Stone');
![output](screenshots/output-week1/insert-section.png)

#insertion into grade_report
INSERT INTO GRADE_REPORT VALUES(17,112,'B');
INSERT INTO GRADE_REPORT VALUES(17,119,'C');
INSERT INTO GRADE_REPORT VALUES(8,85,'A');
INSERT INTO GRADE_REPORT VALUES(8,92,'A');
INSERT INTO GRADE_REPORT VALUES(8,102,'B');
INSERT INTO GRADE_REPORT VALUES(8,135,'A');
![output](screenshots/output-week1/insert-gradereport.png)

#table of student
SELECT * FROM student;
![output](screenshots/output-week1/1-table.png)

#table of course
SELECT * FROM course;
![output](screenshots/output-week1/2-table.png)

#table of section
SELECT * FROM section;
![output](screenshots/output-week1/3-table.png)

#table of grade_report
SELECT * FROM grade_report;
![output](screenshots/output-week1/4-table.png)
