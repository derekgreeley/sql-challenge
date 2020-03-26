DROP TABLE departments;

CREATE TABLE departments(
	dept_no VARCHAR(4) NOT NULL,
	dept_name VARCHAR(30) NOT NULL
);

DROP TABLE dept_emp;

CREATE TABLE dept_emp(
	emp_no INT SERIAL PRIMARY KEY, 
	dept_no VARCHAR(4) NOT NULL,
	from_date VARCHAR(10),
	to_date VARCHAR(10),
);

DROP TABLE dept_manager;

CREATE TABLE dept_manager(
	emp_no INT SERIAL PRIMARY KEY,
	dept_no VARCHAR(4) NOT NULL,
	from_date VARCHAR(10),
	to_date VARCHAR(10),
);

DROP TABLE employees;

CREATE TABLE employees(
	emp_no INT SERIAL PRIMARY KEY,
	birth_date VARCHAR(10),
	first_name VARCHAR(20),
	last_name VARCHAR(20),
	gender VARCHAR(12),
	hire_date VARCHAR(10)
);

DROP TABLE salaries;

CREATE TABLE salaries(
	emp_no INT SERIAL PRIMARY KEY,
	salary INT,
	from_date VARCHAR(10),
	to_date VARCHAR(10),
);

DROP TABLES titles;

CREATE TABLES titles(
	emp_no INT SERIAL PRIMARY KEY,
	title VARCHAR(30),
	from_date VARCHAR(10),
	to_date VARCHAR(10),
);


