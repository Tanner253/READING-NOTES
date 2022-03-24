# Data modeling

## noSQL vs SQL

- SQL databases are known as 'relational' databases. NoSQL Databases are not relational. What this means is that a table in a SQL database might have a connection to another table in the database for referencing attatched data. this allows us to organize each type of data in its own tables for scalability, and organization, and debugging. Whereas NoSQL database contains all of its data in a document which may have inconsistent collumns or data. SQL databases have a predefined schema and a vertically scaleable while nosql databases do not have a predefined schema, and scale horizontally (collumns)

  - SQL databases are better for complex querying.

## SQL modeling techniques

![data model example](../../Assets/example.png)

Data modeling is the action of diagaming out the tables in a database and how they relate to eachother (does a table have a 1 to 1 connection or a 1 to many connection?) for example a customer has 1 cart, but a car can have many items. so the customer has a 1 to 1 with the cart, and the cart has a 1 to many with products. things that should be in the diagram is the appropriate table name, PK, FK, and table collumns.