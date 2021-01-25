# SQL-For-Fun
Basic SQL queries.

SQL, which stands for `Structured Query Language`, is a language for interacting with data stored in something called a relational database.

You can think of a relational database as a collection of tables. A table is just a set of rows and columns, like a spreadsheet, which represents exactly one type of entity.

Each row, or record, of a table contains information about a single entity. Each column, or field, of a table contains a single attribute for all rows in the table.

### Basic Queries:
#### 1. SELECTing single columns


While SQL can be used to create and modify databases, the focus of this course will be querying databases. A query is a request for data from a database table (or combination of tables). Querying is an essential skill for a data scientist, since the data you need for your analyses will often live in databases.

In SQL, you can select data from a table using a SELECT statement. For example, the following query selects the name column from the people table:

```SELECT name
FROM people;```
In this query, SELECT and FROM are called keywords. In SQL, keywords are not case-sensitive, which means you can write the same query as:

```select name
from people;```
That said, it's good practice to make SQL keywords uppercase to distinguish them from other parts of your query, like column and table names.

It's also good practice to include a semicolon at the end of your query. This tells SQL where the end of your query is!

#### 2. SELECTing multiple columns
Well done! Now you know how to select single columns.

In the real world, you will often want to select multiple columns. Luckily, SQL makes this really easy. To select multiple columns from a table, simply separate the column names with commas!

For example, this query selects two columns, name and birthdate, from the people table:

```SELECT name, birthdate
FROM people;```
Sometimes, you may want to select all columns from a table. Typing out every column name would be a pain, so there's a handy shortcut:

```SELECT *
FROM people;```
If you only want to return a certain number of results, you can use the LIMIT keyword to limit the number of rows returned:

```SELECT *
FROM people
LIMIT 10;```


