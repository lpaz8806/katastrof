# katastrof
Inlämningsuppgift's cousin project to make the babies to cool down a bit :)

## Project Specification
Katastrofhoet AB is having issues with the staff. They fail to remember the tasks to be done and
productivity is going down, so the managers are willing to take immediate action. We are ordered
to build an application to manage the tasks.

From `users`, we want to know the `username` for login purposes, no longer than 64
characters. We also want to know the `email` and the `name`, which must be no longer than 50
characters.

From `todos`, we want to know a `description`, which will be no longer than 200 characters, an
optional `due_date`, a boolean flag `is_done`, a boolean flag `is_important`.

Todos may be grouped into `todo_lists`. We want to know the `name` of the list, which is a
string of at most 64 characters. We want to know the `user` who owns the list. One user can
create many todo_lists. One todo_list can contain many todos and one todo may be in at
most one todo_list.

Todo_lists can be "shared" between users. One todo_list can be shared with many users and
one user can have many todo_lists shared

When a todo_list is removed, the todos it contains are not destroyed.

## Vad ska ni göra

### Test
The testing team is responsible for creating unit tests that make sure that:
1. Every entity (table) has a primary key
2. Every primary key is called id
3. Foreign key constraints are enforced on each relationship
4. Every column type matches the type specified above

### Dev
The development team is responsible for:
1. Creating the database schema in “src/sql/db.schema.sql”
2. Create all the necessary tables, foreign	keys constraints, etc. to model the specified problem. The code	with will 
be written also in “src/sql/db.schema.sql”
