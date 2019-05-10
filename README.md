# Importing a large database in MAMP

If you try to import a database over 32mb you might run into some problems. phpMyAdmin has a few suggestions in the docs but for the sake of uploading one file it is much easier to use Terminal to add our big old database.

- Start MAMP
- Start the server
- Open Terminal and enter the below

```
/Applications/MAMP/Library/bin/mysql --host=localhost -uroot -proot
```

Now you can use the MySQL command line

To connect to your database

```
connect your_database_name
```

To import your database

```
source /path/to/your/file/sql_export.sql
```

Give MYSQL some time to do its thing. 

All done. 

## Bonus tip

If you would like to see all your databases type:

```
show databases;
```
