## Real world database

Based on different data to store, storage method and database building method, there are two main database kinds:

- SQL (relational database)
- NoSQL (non-relational databases)

## SQL

Relational database store data in columns and rows. Such as MySQL, Oracle, MS SQL Server, SQLite, Postgres, and MariaDB.

## NoSQL

Main features of NoSQL:

1. **Key-Value Stores:** Data is stored in an array of key-value pairs. Such as Redis, Voldemort, and Dynamo.
2. **Document database:** Data is stored in document instead of columns and rows and these documents are grouped together in collections. Document databases include the CouchDB and MongoDB.
3. **Wide-Column Databases:** It is not necessary to know all the columns up front and each row doesn’t have to have the same number of columns. Columnar databases are best suited for analyzing large datasets - big names include Cassandra and HBase.
4. **Graph Databases:** Data is saved in graph structures with nodes (entities), properties (information about the entities), and lines (connections between the entities). Examples of graph database include Neo4J and InfiniteGraph.

## Differences between SQL and NoSQL

1. **Storage**
   - SQL: Store data in tables and each column and row can represent a data point.
   - NoSQL: Storing large volumes of data which might not be structured. NoSQL databases set no limites on data types and store them all together. We don't have to change anything even if we have new data type to store. With document-based database, we can store data without defining data type in advance.
2. **Schema**
   - SQL: The schema is static. Each record conforms to a fixed schema, which means columns must be decided before data entry and each row must have value for each column. The schema can be altered later; however, it would involves the whole dataset changing.
   - NoSQL: The schema is dynamic. Columns can be added on the fly and each row doesn't have contain each column.
3. **Querying**
   - SQL: Using SQL (structured query language) for manipulating data.
   - NoSQL: Queries are focused on a collection of documents and is called UnQL (unstructured query language). Different stored data types have different syntax for using UnQL.
4. **Scalability**
   - SQL: Vertically scalable. 
   - NoSQL: Horizontally scalable, meaning we can add more servers easily in NoSQL database infrastructure to handle a lot of traffic. Any cheap hardware can host NoSQL database and thus making it a lot more cost-effective than vertical scaling. For example, Cassandra are designed to be scaled across multiple data centers out of the box, without a lot of headaches.
5. **Reliability or ACID Compliancy (Atomicity, Consistency, Isolation, Durability)**
   - SQL: Most of relational database are ACID compliant.
   - NoSQL: Most of the NoSQL solutions sacrifice ACID compliance for performance and scalability.
