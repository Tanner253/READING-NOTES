# Mongo / mongoos
Differences between:
SQL \ \ \ 	NoSQL
-verticle  \ \ \ horizontal
- high support from vendors \ \ \ community based suport
-ACID  \ \ \ CAP
-single queries work well   \ \ \ good for large datasets like json 
- What kind of data is a good fit for an SQL database?

>SQL databases are Table based, so organized data that can be accessed with table key values. This is ideal for complex querying.

- Give a real world example.

>User accounts, Product CMS, high transactional dabases SQL is more stable

- What kind of data is a good fit a NoSQL database?

>horizontally scalable where SQL databases are vertically scalable

- Give a real world example.

>adding another server to handle traffic

- Which type of database is best for hierarchical data storage?

>noSQL

- Which type of database is best for scalability?

>SQL

- What does SQL stand for?

>Structured query language

- What is a relational database?

>clear schema, SQL database

- What type of structure does a relational database work with?

>Tables, Fields(collumns) many to many relations, 1 to 1 many to 1 or 1 to many

- What is a ‘schema’?

>the blueprint for the tables and database of the whole

- What is a NoSQL database?

>non relational database

- How does it work?

>collections and documents, look like json, noSQL doesnt have to use the same schema, theres no schema. where objects can have unique "collumns"

- What is inside of a Mongo database?

>(see above)

- Which is more flexible - SQL or MongoDB? and why.

>mongodb bc you have far more flexibility adding new data or rendering data

- What is the disadvantage of a NoSQL database?

>no relations (Explicitley) duplicated data, wastes space when writing a lot inserts.