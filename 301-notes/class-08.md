# Structured Query Language (SQL)

**Links:**
[SQLBolt](https://sqlbolt.com/)
[W3School Practice](https://www.w3schools.com/sql/trysql.asp?filename=trysql_select_all)
[SQL Cheat Sheet](http://www.cheat-sheets.org/sites/sql.su/)

## What is SQL?

SQL, or Structured Query Language, is a language designed to allow both technical and non-technical users query, manipulate, and transform data from a relational database. And due to its simplicity, SQL databases provide safe and scalable storage for millions of websites and mobile applications.


A relational database represents a collection of related (two-dimensional) tables. Each of the tables are similar to an Excel spreadsheet, with a fixed number of named columns (the attributes or properties of the table) and any number of rows of data.

### SQL SELECT queries

To retrieve data from a SQL database, we need to write SELECT statements, which are often colloquially refered to as queries. A query in itself is just a statement which declares what data we are looking for, where to find it in the database, and optionally, how to transform it before it is returned. 


```SQL
SELECT column, another_column, …
FROM mytable;
```


If we want to retrieve absolutely all the columns of data from a table, we can then use the asterisk (*) shorthand in place of listing all the column names individually.

```SQL
SELECT * 
FROM mytable;
```

### Queries with constraints

In order to filter certain results from being returned, we need to use a **WHERE** clause in the query. The clause is applied to each row of data by checking specific column values to determine whether it should be included in the results or not.

```sql
SELECT column, another_column, …
FROM mytable
WHERE condition
    AND/OR another_condition
    AND/OR …;
```


