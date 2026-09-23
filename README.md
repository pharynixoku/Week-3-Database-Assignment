1--CREATing  student Table
CREATE TABLE student (
    id INT PRIMARY KEY,
    fullName VARCHAR(100),
    age INT
);

CREATE TABLE — tells SQL that we want to create a new table.
student — the name of the table.
id — the column used to identify each student.
INT — means the value must be a whole number, such as 1, 2, or 20.
PRIMARY KEY — makes id unique for each student. Two students cannot have the same ID.
fullName — stores the student's full name.
VARCHAR(100) — stores text with a maximum of 100 characters.
age — stores the student's age.
; — indicates the end of the SQL statement.


2--Inserting the id,full name,and age in to student table
INSERT INTO student (id, fullName, age)
VALUES
    (1, 'Simon Ohure', 19),
    (2, 'Okuu Sooa', 18),
    (3, 'Peter James', 21);

INSERT INTO — tells SQL that we want to add data to a table.
student — specifies the table where the data will be added.
(id, fullName, age) — specifies the columns receiving the data.
VALUES — introduces the actual information being inserted.
(1, 'Simon Ohure', 19) — creates the first student.
(2, 'Okuu Sooa', 18) — creates the second student.
(3, 'Peter James', 21) — creates the third student.
Text values such as names are placed inside single quotation marks 


3-- Updating is to change some information in student table
UPDATE student
SET age = 20
WHERE id = 2;

UPDATE student — tells SQL that we want to change information in the student table.
SET age = 20 — changes the student's age to 20.
WHERE id = 2 — tells SQL which student should be updated.
; — ends the statement.
