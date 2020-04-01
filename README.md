# In-class command examples

-- CREATE TABLE <table name> (
--   <column name> <datatype> <constraints..>,
--   <column name> <datatype> <constraints..>,
--   <column name> <datatype> <constraints..>
-- );

-- STUDENT TABLE
-- student_id	NAME TEXT       AGE iNT
--  1 					eric						NULL
--  2 						eric						29
--  3 								erik						12

--  5 						melissa
--  6 						melissa
--  7						kyle							74

 
-- CREATE TABLE user_option (
--   user_options_id SERIAL PRIMARY KEY, 
--   dark_mode BOOL,
--   fav_num INTEGER,
--   fav_dec FLOAT,
--   fav_dec2 DECIMAL,
--   fav_word TEXT,
--   fav_short_word VARCHAR(5)
-- );

-- CREATE TABLE student (
--   student_id SERIAL PRIMARY KEY,
--   first_name VARCHAR(255) NOT NULL,
--   last_name VARCHAR(255),
--   lines_of_code_written INTEGER,
--   first_time_coding TEXT
-- );

-- INSERT INTO student (first_name, last_name, lines_of_code_written, first_time_coding)
-- VALUES ('Charlie', 'Pan', 10, 'High School');

-- INSERT INTO student (first_name, last_name, lines_of_code_written, first_time_coding)
-- VALUES ('Trevor', 'Ramey', 11, 'High School'),
-- 			('Jordan', 'Morris', 2000, 'High School'),
--   		('Jeremy', 'Laningham', 13, '2019');

-- INSERT INTO student (first_name, last_name)
-- VALUES ('Daniel', 'Reyes');

-- UPDATE student
-- SET lines_of_code_written = 1000000
-- WHERE student_id = 6;

-- UPDATE student
-- SET first_time_coding = '1972';


-- WHERE lines_of_code_written != 13 AND first_name != 'Charlie';

-- INSERT INTO student (first_name, lines_of_code_written)
-- VALUES ('Melissa', 10000);

-- SELECT * FROM student
-- WHERE last_name IS NOT NULL;

-- SELECT * FROM artist
-- OFFSET 10
-- LIMIT 10;

-- CREATE TABLE student_city (
--   student_city_id SERIAL PRIMARY KEY,
--   student_id INTEGER REFERENCES student(student_id),
--   city TEXT
-- )

-- SELECT * FROM student
-- WHERE first_name ILIKE 'charlie';

SELECT * FROM student
WHERE last_name LIKE '%an%';

-- SELECT * FROM student;


