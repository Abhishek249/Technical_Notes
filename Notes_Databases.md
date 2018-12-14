https://www.guru99.com/sql-interview-questions-answers.html

The person expecting--
30 min


What is DBMS?

What are DDL, DML, SQL?

Whare are Logical, physical and user layer of DB design?


What is data independence?


What is table schema?


What do you mean by relational?


--Joins
    https://www.essentialsql.com/get-ready-to-learn-sql-12-introduction-to-database-joins/
    https://www.deskbright.com/sql/sql-joins-interview-questions/
    https://academy.vertabelo.com/blog/introduction-using-aggregate-functions-joins/ 
    Table joins are used to extract information from 2 or more tables by specifying a join condition which acts as the basis of 
    relationship between records of those tables. Inherently under the principles of DB, the tables are created in a way to follow
    Normalization principles which are enforced to eliminate update anomalies. 
    So, to extract information for analytical purposes,we need to collect information from multiple tables and this is done using
    JOINS. 

    Types of JOINS:-
    - INNER JOIN

    - OUTER JOIN

    - CROSS JOIN

--Indexes
    https://www.toptal.com/sql-server/sql-database-tuning-for-developers
    https://www.essentialsql.com/what-is-a-database-index/
    https://www.geeksforgeeks.org/indexing-in-databases-set-1/
    https://www.sitepoint.com/using-explain-to-write-better-mysql-queries/

    An INDEX is a data structure that improves the speed of data retrieval operations on a database table by providing rapid lookups
    and efficient access to ordered records.
    Indexes are also used to define a primary key or unique index which will guarantee that no other columns have the same values.
    **Difference between UNIQUE and PRIMARY key
        Primary Key:
            There can only be one primary key in a table
            In some DBMS it cannot be NULL - e.g. MySQL adds NOT NULL
            Primary Key is a unique key identifier of the record
        
        Unique Key:
            Can be more than one unique key in one table
            Unique key can have NULL values
            It can be a candidate key
            Unique key can be NULL and may not be unique

    *Types of Indexes:-
    -



--Normalization:-
    https://www.essentialsql.com/get-ready-to-learn-sql-database-normalization-explained-in-simple-english/
    Normalization is a process of restructuring a relational database in accordance with a series of rules called NORMAL FORMS in order
    to reduce data redundancy and improve data integrity.
    The basic idea is to make a table "single purpose specific" and to include only those columns that support that purpose.
    e.g. an academic database containing student information:
    -- StudentID | StudentName |  StudentPhone |    Class1 |  Class2 |  Class3
    -- it is a bad design
     

-- Stored Procedures


-- Views

-- Peformance Tuning in Databases and Query Optimization
    https://technet.microsoft.com/en-us/library/ms172984(v=sql.110).aspx