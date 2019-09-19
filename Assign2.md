Assignment 2
------------
Create a simple schema with referential integrity constraints (foreign keys) and uniqueness constraints (primary keys and additional unique indexes)

1. Complete the definition of the Enrollment database presented in class: [presentation](Enroll.pdf) and [notebook](https://nbviewer.jupyter.org/github/msds-5315/Database-Systems-for-Data-Science/blob/master/notebooks/Enroll.ipynb)

2. Insert several records in each table (at least 10 in `Person`, at least 4 in `Course`, at least 8 in `Section`, at least 30 in `Enroll`)

3. Modify the table `Section` so that the table its `instructor` field should only contain valid `person_id`s from `Person`. To modify a table, you should use the `DROP TABLE` command and `CREATE TABLE` again with the new definition.

4. Produce an `INSERT` statement that violates a foreign key constraint and is prevented by the database.

5. Produce a `DELETE` statement that violates a foreign key constraint and is prevented by the database.

6. Extend the database to represent textbooks selected for each entry in `Section`. Each textbook entry should contain its ISBN, title, author, publisher, and publication year. Assume that each section has exactly one textbook.
