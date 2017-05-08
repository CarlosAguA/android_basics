# Running SQLite on computer

Once SQLite was succesfully installed, the library must be opened from the command line.

![](/assets/command_sqlite.png)

Once this screen appears on your computer it means that you can succesfully open sqlite on it.

### Designing and creating database on the computer

The first thing to do is sketching the content of the db with the name of the table as well as the data type. Doing so will make the process so much easier to avoid any mistake. In the course, you interact with the shelter database and the pets and headphones tables. An example mixing those is used just to show how to use the commands to create a design the db.

* Opening db : `sqlite3 pets.db`

* Creating a table : `CREATE TABLE headphones(_id INTEGER, price INTEGER, style INTEGER, in_stock INTEGER, description TEXT);`

* Checking the tables in a db : `.tables`

* Checking how the db was created : `.schema headphones`

* Visualizing the table´s content: `PRAGMA TABLE_INFO(headphones);`

* Delete table : `DROP TABLE headphones;`

### SQlite commands

**sqlite3 :** Command to open up the sqlite3 program in the Command Prompt.

**sqlite3 shelter.db :** Command to open up the sqlite3 program and directly open up the following database file. You can substitute shelter.db for any other existing database file.

**.open shelter.db :** Command inside the sqlite program to open a database file. In this case we are opening the shelter.db file. You can substitute any other existing .db file for shelter.db

**.help :** Command to pint out a list of available commands.

**.quit :** Command to quit the sqlite application.





