Here, I will disuss step by step to proseed with the postgreSQL on [freecodecamp.org](https://www.freecodecamp.org/fcc7011b5c1).

## Step-1: Login
```
codeally@147a091d400c:~/project$ psql --username=freecodecamp --dbname=postgres
```
Output will be
```
Border style is 2.
Title is " ".
Pager usage is off.
psql (12.9 (Ubuntu 12.9-2.pgdg20.04+1))
Type "help" for help.
```
Now terminal will be converted to

```
postgres=>
```
## Step-2: Check content of the filess in the directory

```
postgres=> \l

```
Output:

```
                               List of databases
+-----------+----------+----------+---------+---------+-----------------------+
|   Name    |  Owner   | Encoding | Collate |  Ctype  |   Access privileges   |
+-----------+----------+----------+---------+---------+-----------------------+
| postgres  | postgres | UTF8     | C.UTF-8 | C.UTF-8 |                       |
| template0 | postgres | UTF8     | C.UTF-8 | C.UTF-8 | =c/postgres          +|
|           |          |          |         |         | postgres=CTc/postgres |
| template1 | postgres | UTF8     | C.UTF-8 | C.UTF-8 | =c/postgres          +|
|           |          |          |         |         | postgres=CTc/postgres |
+-----------+----------+----------+---------+---------+-----------------------+
```
## Step-3: Creeating aa database

The databases you see are there by default. You can make your own like this:
```
postgres=> CREATE DATABASE first_database
```
The capitalized words are keywords telling PostgreSQL what to do. The name of the database 
is the lowercase word. Note that all commands need a semi-colon at the end. Create a new database named `first_database`.




