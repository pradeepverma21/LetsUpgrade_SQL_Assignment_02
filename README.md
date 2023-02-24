# LetsUpgrade_SQL_Assignment_02

Create a table called "students" with columns "id" (integer, primary key, auto-increment), "name" (text), "age" (integer), and "gender"

(text).

1.Insert three rows of data into
the "students" table.

2.Retrieve all rows from the "students" table.

3.Update the name of the student with id = 2 to "Janet".

4.Delete the row with id = 3 from the "students" table.

5.Retrieve all rows from the "students" table again to verify that the changes have been made.



-- Create the "students" table
CREATE TABLE students (
  id INTEGER PRIMARY KEY AUTOINCREMENT,
  name TEXT,
  age INTEGER,
  gender TEXT
);

-- Insert three rows of data into the "students" table :
INSERT INTO students (name, age, gender) VALUES ('Alice', 21, 'Female');
INSERT INTO students (name, age, gender) VALUES ('Bob', 22, 'Male');
INSERT INTO students (name, age, gender) VALUES ('Charlie', 23, 'Male');

-- Retrieve all rows from the "students" table :
SELECT * FROM students;

-- Update the name of the student with id = 2 to "Janet" : 
UPDATE students SET name = 'Janet' WHERE id = 2;

-- Delete the row with id = 3 from the "students" table :
DELETE FROM students WHERE id = 3;

-- Retrieve all rows from the "students" table again to verify that the changes have been made :
SELECT * FROM students;
