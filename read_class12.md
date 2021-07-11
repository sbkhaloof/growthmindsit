# Mongo and Mongoose
## nosql vs sql

1. Fill in the chart below with five differences between SQL and NoSQL databases


|                    SQL                                |                                    NOSQL                            |
|------------------------------------------------------ |:------------------------------------------------------------------: |
| primarily called as Relational Databases (RDBMS)      |         called as non-relational or distributed database.           |
|                 table based databases                 |document based,key-value pairs,graph databases or wide-column stores.|     
|              have predefined schema                   |           dynamic schema for unstructured data.                     |
|                 vertically scalable                   |                       horizontally scalable.                        |
|              structured query language                |                     Unstructured Query Language                     |
| examples: MySql, Oracle, Sqlite, Postgres and MS-SQL. |examples: MongoDB, BigTable, Redis, RavenDb, Cassandra, Hbase, Neo4j |


1. What kind of data is a good fit for an SQL database?
####  SQL databases are good fit for the complex query intensive environment whereas NoSQL databases are not good fit for complex queries. On a high-level, NoSQL don’t have standard interfaces to perform complex queries, and the queries themselves in NoSQL are not as powerful as SQL query language.
2. Give a real world example.
####  SQL database MS-SQL 
3. What kind of data is a good fit a NoSQL database?
#### NoSQL database are good fit and better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data.
4. Give a real world example.
#### Mongodb
5. Which type of database is best for hierarchical data storage?
#### SQL databases are not best fit for hierarchical data storage. But, NoSQL database fits better for the hierarchical data storage 
6. Which type of database is best for scalability?
#### SQL databases are vertically scalable. You can manage increasing load by increasing the CPU, RAM, SSD, etc, on a single server. On the other hand, NoSQL databases are horizontally scalable. You can just add few more servers easily in your NoSQL database infrastructure to handle the large traffic.

## sql vs nosql (Video)

1. What does SQL stand for?
#### Structured Query Language
2. What is a realational database?
#### A relational database is a type of database that stores and provides access to data points that are related to one another. Relational databases are based on the relational model, an intuitive, straightforward way of representing data in tables. In a relational database, each row in the table is a record with a unique ID called the key. The columns of the table hold attributes of the data, and each record usually has a value for each attribute, making it easy to establish the relationships among data points.
3. What type of structure does a relational database work with?
#### the data tables, views, and indexes
4. What is a ‘schema’?
#### a logical collection of database objects.
5. What is a NoSQL database?
#### not only SQL 
6. Howo does it work?
#### databases do not rely on these structures and use more flexible data models. NoSQL can mean “not SQL” or “not only SQL.” As RDBMS have increasingly failed to meet the performance, scalability, and flexibility needs that next-generation, data-intensive applications require, NoSQL databases have been adopted by mainstream enterprises. NoSQL is particularly useful for storing unstructured data, which is growing far more rapidly than structured data and does not fit the relational schemas of RDBMS. Common types of unstructured data include: user and session data; chat, messaging, and log data; time series data such as IoT and device data; and large objects such as video and images.
7. What is inside of a Mongo database?
#### document stored in a collection
8. Which is more flexible - SQL or MongoDB? and why.
#### MongoDB
9. What is the disadvantage of a NoSQL database?
#### when you want to update a spcific data, you have to update all collections that contain that data.


