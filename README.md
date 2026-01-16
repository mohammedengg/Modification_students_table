# Students Table – Data Types & Constraints

## Tools Used
- MySQL Workbench
- MySQL Server

## Task Description
This task focuses on redesigning an existing `students` table by applying
proper SQL data types, constraints, and table modification commands to
ensure data integrity.

## Initial Table Structure
The table initially contained the following columns:
- id (INT)
- name (VARCHAR)
- email (VARCHAR)
- age (INT)

Sample data was inserted before applying constraints.

## Constraints Applied
- PRIMARY KEY on `id` to uniquely identify each student
- AUTO_INCREMENT on `id` for automatic ID generation
- NOT NULL on `full_name` and `email` to prevent missing data
- UNIQUE on `email` to avoid duplicate student records
- CHECK constraint on `age` to prevent invalid values

## Table Modifications
- Added a new column `date_of_birth` using ALTER TABLE
- Renamed column `name` to `full_name`
- Dropped column `age` and documented its consequences

## Constraint Testing
Invalid data insertions were attempted to verify:
- UNIQUE constraint failure
- NOT NULL constraint failure
- CHECK constraint failure

## Final Table Structure
- id
- full_name
- email
- date_of_birth

## Conclusion
Constraints are essential for maintaining data accuracy, consistency,
and reliability by enforcing rules directly at the database level.
