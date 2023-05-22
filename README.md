# THEORIES
1. What is Database (DB)?
2. How to create Database?
3. What is Database Management System (DBMS)?
4. What to learn?
    + Database Design
    + Interact
    + Data Science
5. [Data types](https://www.postgresql.org/docs/current/datatype.html)
6. Keys
    + Primary Key
    + Foreign Key
# INSTALATION
This is the instalation method using packages
1. Visit postgresql download [link](https://www.postgresql.org/download/)
2. Select your operating system
3. Set password
4. Do not open Stack Builder
5. (For Window users only) Add the PostgreSQL bin directory path to the PATH environmental variable  
6. Open the command-line tool
    + Test instalation: 
    ```bash
    psql --version
    ```
    + Log in and enter password
    ```bash
    psql -U postgres
    ```
7. Type "exit" two times to close command prompt
# USAGE
1. SQL querry: 

    ## Documents
    + [The ANSI standard syntax](https://blog.ansi.org/2018/10/sql-standard-iso-iec-9075-2016-ansi-x3-135/#gref)
    + [PostgreSQL Documentation](https://www.postgresql.org/docs/)

    ## Tools
    + Command Line
    + GUI: PgAdmin
    ## CRUD Action
    + Create   
        + Database
        ```SQL
        CREATE DATABASE database_name;
        ```
        + Table
        ```SQL
        CREATE TABLE table_name (
            var     type    constraints     key_or_not
        );
        ```
        + Insert a record
        ```SQL 
        INSERT INTO table_name (
            col_nameyour_db
        ) VALUE ('value');
        ```
    + Retrieve
        ```SQL
        SELECT col_name FROM table_name;
        ```
        + DISTINCT(col_name)
        + ORDER BY col_name ASC/DESC
        + WHERE condition (AND/OR/NOT)
        + LIMIT
        + JOINS
    + Update
        ```SQL
        UPDATE your_table SET col_name = col_value (WHERE ...);
        ```
    + Delete
        + Records: Use primary key
        ```SQL
        DELETE FROM table_name (WHERE ...);
        ```
        + Table
        + Database
        ```SQL
        DROP DATABASE database_name;
        ```
2. Code: Python
    + Libraries Usage
    + Data Access Object (DAO)
    + ORM
    + Example: https://github.com/hieuduy6098/sqliteAccessLib

# QUESTIONS
1. Why do we need a semicolon at the end of each query?
# REFERENCES
1. [NoSQL vs SQL – Which Type of Database Should You Use?](https://www.youtube.com/watch?v=FzlpwoeSrE0)
1. [Learn PostgreSQL Tutorial - Full Course for Beginners](https://www.youtube.com/watch?v=qw--VYLpxG4)