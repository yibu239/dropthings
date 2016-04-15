# Problem #

Create a new database in SQL Server 2005 or 2008 manually without using the attached .mdf.


# Solution #

There's a install.sql file in \trunk\deploy\DropthingsPacakge folder.

You need to change the following lines:

```
-- Set variables for database name, username and password
SET @dbName = 'PlaceHolderForDb';
SET @dbUser = 'PlaceHolderForUser';
SET @dbPwd = 'PlaceHolderForPassword';
```

Then run this script and it will create a new database for you.