# Database Tutorial 


#### Database Commands

##### Show Database
To see the databases are present with help of this commands we can see. 

```sql 
  show databases;
```

##### Create Database

```sql
    create database database_name;
```

##### Drop Database

```sql
    drop database databaseName; 
```

##### Change Database 

```sql
    use databaseName; 
```

#### Tables Commands

    A collection of the related data held in structural format within a database. 
    Databases are made of lots of the tables. 

##### DataTypes in Tables

###### Numeric DataType 
  - INT 
  - SMALLINT
  - TINYINT 
  - MEDUIMINT
  - BIGINT
  - DECIMAL
  - NUMERIC 
  - FLOAT 
  - DOUBLE 
  - BIT 

###### String DataType  
  - CHAR 
  - VARCHAR
  - BINARY 
  - VARBINARY
  - BLOB
  - TINYBLOB
  - MEDUIMBLOB
  - LONGBLOB
  - TEXT
  - TINYTEXT

 ##### Create Tables

 ```sql
     create table Name_Table (
        prop1 type,
        prop2 type, 
        prop3 type 
     ); 

     /* Example */
     create table student (
        Id int,
        Name varchar(15),
        Age int
     );
 ``` 

##### Tables Related Commands

- Show Table  

```sql
    show tables; 
```

This commands will show all the tables inside database


- Show columns details

```sql
    show columns from tableName; 
```

This command will show the column name and datatype of the column. 


- Describe table 

    Describe table is same as the above commands

```sql
    describe tableName; 
    /*OR*/
    desc tableName;
```

- Delete the tables 

```sql
    drop table tableName; 
```


- Insert Into tables
```sql
    Insert into tableName(prop1, prop2) Values  ("val1", "val2");
    -- Example 
    Insert into student(Id, name, age) values (1,"Jon",2);

    -- Insert Multiples values 

    Insert into student(Id, name, age) values (1,"Jon",2),(2,"Bob",3),,(3,"Insta",4); 
```

- Select Command

```sql
    select * from table_Name;

    -- to select specific columns
    
    select col1, col2, col3 from tableName;
```

##### Constraint in SQL 

 - NOT NULL

 ```sql
 
 create table tableName(prop1 type not null, prop2 type not null); 

 -- example

 create table student(name varchar(20) not null, age int not null);
 
 ``` 

 - DEFAULT 

    It is used to give the default value of the column
```sql
create table student(name varchar(20) defualt 'surya' not null, age int not null);

```
