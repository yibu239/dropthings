# Introduction #

Dropthings uses an N-tier architecture with clear separation of data and business logic. See how to introduce a new business operation in the business layer and make it call a data access layer operation and how to create a new Linq to SQL compiled query.


# Details #

Watch this screencast:

http://omaralzabir.com/wp-content/movies/AddNewBusOp.html

# UPDATE #
From version 2.6, the data access layer has been converted to Entity Framework. So, you will have to follow the entity framework way of writing compiled queries and use the new DropthingsDataContext2 to do CRUD. Read this article for details on working with Entity Framework in a N-tier application.

http://www.codeproject.com/KB/linq/ef.aspx