# PostgreSQL university
> The task was completed as part of the Python Core course at GoIT.

## Table of Contents
* [General Info](#general-information)
* [Setup](#setup)
* [Project Status](#project-status)


## General Information
The database filled with random data (~30-50 students, 3 groups, 5-8 subjects, 3-5 teachers, up to 20 grades for each student across all subjects). Faker package used for data generation.


## Setup

Database with the following schema:

- Student table;
- Group table;
- Teacher table;
- Subject table indicating the teacher who teaches the subject;
- Table where each student has grades for subjects with the date the grade was received.

Perform the following queries on the database:

Find the top 5 students with the highest average grade across all subjects.

 Find the student with the highest average grade in a specific subject.
 
 Find the average grade in groups for a specific subject.
 
 Find the average grade in the stream (across the entire grade table).
 
 Find which courses a specific teacher teaches.
 
 Find the list of students in a specific group.
 
 Find the grades of students in a specific group for a specific subject.
 
 Find the average grade given by a specific teacher across their subjects.
 
 Find the list of courses attended by a student.
 
 List of courses taught by a specific teacher to a specific student.



For each query, create a separate file named query_number.sql, where number is replaced by the query number. The file should contain the SQL instruction that can be executed either through the database terminal or via cursor.execute(sql).


## Project Status
Project completed: Oct 6, 2023
