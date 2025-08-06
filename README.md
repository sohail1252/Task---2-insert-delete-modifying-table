CREATE TABLE students (
    id INT PRIMARY KEY,
    name VARCHAR(100),
    age INT DEFAULT 18,
    grade VARCHAR(5)
);


INSERT INTO students (id, name, age, grade)
VALUES (1, 'Alice', 20, 'A');


INSERT INTO students (id, name, grade)
VALUES (2, 'Bob', 'B');


INSERT INTO students (id, name, age, grade)
VALUES (3, 'Charlie', 21, NULL);

UPDATE students
SET grade = 'A+'
WHERE id = 2;


DELETE FROM students
WHERE grade IS NULL;


SELECT * FROM students;
