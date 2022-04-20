# dbms viva questions

## what is dbms? ##
## difference between datastructure and database ##
## what is deadlock? ##
## how to resolve deadlock? ##
## what are the four ACID properties ? ##
## what is redudancy? how to resolve that? ##
## what is normalisation ? what are the types of normalisaton ? where it is used ? ##
## what is the difference between primary key and foreign key ? ##
## explain different type of keys in dbms ##
  - Candidate Key: The candidate key represents a set of properties that can uniquely identify a table. Each table may have multiple candidate keys. One key amongst all candidate keys can be chosen as a primary key. In the below example since studentId and firstName can be considered as a Candidate Key since they can uniquely identify every tuple.
  
  - Super Key: The super key defines a set of attributes that can uniquely identify a tuple. Candidate key and primary key are subsets of the super key, in other words, the super key is their superset.

  - Primary Key: The primary key defines a set of attributes that are used to uniquely identify every tuple. In the below example studentId and firstName are candidate keys and any one of them can be chosen as a Primary Key. In the given example studentId is chosen as the primary key for the student table.
  
  - Unique Key: The unique key is very similar to the primary key except that primary keys don’t allow NULL values in the column but unique keys allow them. So essentially unique keys are primary keys with NULL values.
  
  - Alternate Key: All the candidate keys which are not chosen as primary keys are considered as alternate Keys. In the below example, firstname and lastname are alternate keys in the database.
  
  - Foreign Key:  The foreign key defines an attribute that can only take the values present in one table common to the attribute present in another table. In the below example courseId from the Student table is a foreign key to the Course table, as both, the tables contain courseId as one of their attributes.
  
  - Composite Key:  A composite key refers to a combination of two or more columns that can uniquely identify each tuple in a table. In the below example the studentId and firstname can be grouped to uniquely identify every tuple in the table
  
## what is schema ? ##
## difference between sql and no-sql ##
## what is the importance of dbms ##
## what is concurency ##
## deadlock prevantion ##
## generalisation and specialisation ##
## ddl , dml , dcl , tcl  ##
  - DDL(Data Definition Language):  It contains commands which are required to define the database.
    E.g., CREATE, ALTER, DROP, TRUNCATE, RENAME, etc.
  - DML(Data Manipulation Language): It contains commands which are required to manipulate the data present in the database.
    E.g., SELECT, UPDATE, INSERT, DELETE, etc.
  - DCL(Data Control Language):  It contains commands which are required to deal with the user permissions and controls of the database system.
    E.g., GRANT and REVOKE.
  - TCL(Transaction Control Language):  It contains commands which are required to deal with the transaction of the database.
    E.g., COMMIT, ROLLBACK, and SAVEPOINT.
## syntax of sql queries ##
## what is rollback? ##
## what is data dictionary? ##
## What is a Join? List its different types. ##
![image](https://user-images.githubusercontent.com/72689203/164173117-6a884589-d9f7-4f04-ae3b-ef4e6ad45031.png)

## What is Cursor? ##
  - A database cursor is a control structure that allows for the traversal of records in a database. Cursors, in addition, facilitates processing after traversal, such as retrieval, addition, and deletion of database records. They can be viewed as a pointer to one row in a set of rows.
  - There are two types of cursors:
  - Implicit Cursor:
Oracle automatically creates a cursor while running any of the commands - SELECT INTO, INSERT, DELETE or UPDATE implicitly.
The execution cycle of these cursors is internally handled by Oracle and returns the information and status of the cursor by making use of the cursor attributes- ROWCOUNT, ISOPEN, FOUND, NOTFOUND.
  - Explicit Cursor:
This cursor is a SELECT statement that was declared explicitly in the declaration block.
The programmer has to control the execution cycle of these cursors starting from OPEN to FETCH and close.
The execution cycle while executing the SQL statement is defined by Oracle along with associating a cursor with it.

## List the different types of relationships in SQL. ##
  - One-to-One - This can be defined as the relationship between two tables where each record in one table is associated with the maximum of one record in the other table.
  - One-to-Many & Many-to-One - This is the most commonly used relationship where a record in a table is associated with multiple records in the other table.
  - Many-to-Many - This is used in cases when multiple instances on both sides are needed for defining a relationship.
  - Self-Referencing Relationships - This is used when a table needs to define a relationship with itself.

## Explain the basic structure followed in PL/SQL? ##
  - The basic structure of PL/SQL follows the BLOCK structure. Each PL/SQL code comprises SQL and PL/SQL statement that constitutes a PL/SQL block.
    Each PL/SQL block consists of 3 sections:
  - The optional Declaration Section
  - The mandatory Execution Section
  - The optional Exception handling Section
  
  ```
    [DECLARE]
  --declaration statements (optional)
    BEGIN
  --execution statements
    [EXCEPTION]
  --exception handling statements (optional)
    END;
    
   ```
   
   
   
   
  


