**Create and run your own SQL files**

This Unit is not a teaching Unit. It's main purpose is to allow students to add and run their own SQL code using MySQL.

# University Schema

We have place the university schema and sample data from the Database Systems Concepts textbook 
into a "university" database inside MySQL.  You can find more details about the database in Appendix A.

You can do whatever you like the the MySQL databases in this unit.  

If you need to reset the database to its original state, from within MySQL, simply execute:
```
source /home/codio/workspace/DSC-university-db/reset-create-university.sql
```
and this will delete and create all the sample data in the database.

## Using the `mysql` client
Open up a terminal window from the **Tools->Terminal** menu.

Once the terminal window is open, just type `mysql` into the command line and a new `mysql>` client will start. 

### Running `mysql` statements
The `mysql` client is enabled with all the database and table editing and reading privileges so you can experiment as much as you want.

### Example DML statements:

Data manipulation commands (CRUD) include: 

```sql
SELECT * FROM db_name.table_name;
```

```sql
INSERT INTO table_name (column1,column2,column3,...)
VALUES (value1,value2,value3,...);
```

```sql
UPDATE table_name
SET column1=value1,column2=value2,...
WHERE some_column=some_value;
```

```sql
DELETE FROM table_name
WHERE some_column=some_value;
```

### Sourcing `*.sql` files
The file tree is enabled as well, here, you can edit the `source.sql` file to add SQL statements and `source` it like this: 

```
mysql> source source.sql
```

Or you can create as many `*.sql` files as you want and `source` them as well.

### Creating a new SQL file
To create a new SQL file, please follow these steps.

1. Select the 'File' menu item at the top of this page.
1. Select 'New File' from the drop down menu.
1. In the dialog that appears, locate the 'File Name' field.
1. Enter 'filename.sql' in this field, where 'filename' is a name you choose for your file. 
1. Press 'OK' and a new window will appear where you can start coding.

### Advanced
If you want to have multiple panels open, you can add and close coding panels from the **View->Panels** menu. 

**License**

The MIT License (MIT)

Copyright (c) 2016 Codio

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
