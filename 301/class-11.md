# Reading

[nosql vs sql](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

1. Fill in the chart below with five differences between SQL and NoSQL databases:

    | SQL                                                                                         | NoSQL                                                                                                                                                                                            |
    |---------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | SQL databases are table based databases                                                     | NoSQL databases are document based, key-value pairs, graph databases or wide-column stores                                                                                                       |
    | SQL databases have predefined schema                                                        | NoSQL databases have dynamic schema for unstructured data                                                                                                                                        |
    | SQL databases are vertically scalable                                                       | NoSQL databases are horizontally scalable                                                                                                                                                        |
    | QL databases are scaled by increasing the horse-power of the hardware                       | NoSQL databases are scaled by increasing the databases servers in the pool of resources to reduce the load                                                                                       |
    | SQL databases uses SQL ( structured query language ) for defining and manipulating the data | In NoSQL database, queries are focused on collection of documents. Sometimes it is also called as UnQL (Unstructured Query Language). The syntax of using UnQL varies from database to database. |

2. What kind of data is a good fit for an SQL database?

    SQL databases are good fit for the complex query intensive environment whereas NoSQL databases are not good fit for complex queries. On a high-level, NoSQL don’t have standard interfaces to perform complex queries, and the queries themselves in NoSQL are not as powerful as SQL query language

3. Give a real world example.

    User profile information for apps like Snapchat/Instagram/Netflix etc.

4. What kind of data is a good fit a NoSQL database?

    SQL databases are not best fit for hierarchical data storage. But, NoSQL database fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data. NoSQL database are highly preferred for large data set (i.e for big data). Hbase is an example for this purpose.

5. Give a real world example.

    Analytics, where adding things down the road would require adding columns to say millions/billions of data, which isn't so easy.

6. Which type of database is best for hierarchical data storage?

    SQL

7. Which type of database is best for scalability?

    NoSQL. It doesn't have things like automatic enforcement of referential integrity, transactions, etc. These are all things that are very handy to have for some problems, and which require some interesting techniques to scale outside of a single server (think about what happens if you need to lock two tables for an atomic transaction, and they are on different servers!).

    The DB doesn't have to do all of these complex operations and locking across much of the dataset, so it's really easy to partition the thing across many servers/disks/whatever and have it work really fast.

[sql vs nosql (Video)](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)

1. What does SQL stand for?

    Structured Query Language

2. What is a relational database?

    A relational database is a type of database that stores and provides access to data points that are related to one another

3. What type of structure does a relational database work with?

    Tables, rows, and columns

4. What is a ‘schema’?

    A schema is a cognitive framework or concept that helps organize and interpret information.

5. What is a NoSQL database?

    NoSQL databases are non-relational or distributed databases.

6. How does it work?

    DB has collections, which contain documents, each with its own schema (possibly) and no relations (by default)

7. What is inside of a MongoDB database?

    DB has collections, which contain documents, each with its own schema (possibly) that looks like JSON (key-value pairs).

8. Which is more flexible - SQL or MongoDB? and why.

    If you want flexibility, a NoSQL database can easily be modified without adapting previous data. It's shardable (more easily), and the schema is dynamic.

9. What is the disadvantage of a NoSQL database?

    Less support overall, not ACID based (Atomicity, Consistency, Isoaltion, Durability)

## Things I want to know more about

1. Where do I even begin? There's so much info in here to download I don't even know what I should ask.
