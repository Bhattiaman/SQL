```
-- Create table
CREATE TABLE Teacher (
  id INT,
  marks INT,
  class INT
);

-- Insert values into the Teacher table
INSERT INTO Teacher (id, marks, class) VALUES
(1, 85, 10),
(2, 90, 11),
(3, 78, 9),
(4, 92, 12),
(5, 88, 10);



-- Create table
CREATE TABLE student (
  id INT,
  name VARCHAR(34),
  email VARCHAR(45)
);

-- Insert values into the student table
INSERT INTO student (id, name, email) VALUES
(1, 'Aman', 'amanbhatti105@gmail.com'),
(2, 'Deepak', 'bhattu32@gmail.com'),
(3, 'Vijay', 'fheh@gmail.com'),
(4, 'Vishwas', 'wejrok@gmail.com');

-- Select all records from the student table
-- SELECT * FROM Teacher;
-- SELECT * FROM student;

-- full join function use

-- SELECT * FROM Teacher as t inner join student as s on t.id = s.id;



-- SELECT t.id, t.marks, t.class, s.name FROM Teacher as t join student as s on t.id = s.id ORDER BY t.id DESC;;

SELECT t.id, t.marks, t.class, s.name FROM Teacher as t join student as s on t.id = s.id ORDER BY t.id DESC limit 1;

```
