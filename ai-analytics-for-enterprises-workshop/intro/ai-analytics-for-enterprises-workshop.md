# Introduction

## About This Workshop

This workshop briefly introduces you to the JSON Duality View feature, working with Property Graphs, Vector DB in Oracle Database 23ai Free. You will create a graph from two tables, one containing bank account information, and another containing bank transactions information.  You will then run graph pattern queries in SQL on this graph.   You will find circular payment chains, multi-hop paths between accounts, and more.

### **JSON Duality**

JSON Relational Duality is a landmark capability in Oracle Database 23ai providing game-changing flexibility and simplicity for Oracle Database developers. This breakthrough innovation overcomes the historical challenges developers have faced when building applications, using relational or document models.

“JSON Relational Duality in Oracle Database 23ai brings substantial simplicity and flexibility to modern app dev,” said Carl Olofson, research Vice President, Data Management Software, IDC. “It addresses the age-old object - relational mismatch problem, offering an option for developers to pick the best storage and access formats needed for each use case without having to worry about data structure, data mapping, data consistency, or performance tuning. No other specialized document databases offer such a revolutionary solution.”

JSON Relational Duality helps to converge the benefits of both document and relational worlds. Developers now get the flexibility and data access benefits of the JSON document model, plus the storage efficiency and power of the relational model. The new feature enabling this convergence is JSON Relational Duality View (Will be referred below as Duality View).

Key benefits of JSON Relational Duality:
- Experience extreme flexibility in building apps using Duality View. Developers can access the same data relationally or as hierarchical documents based on their use case and are not forced into making compromises because of the limitations of the underlying database. Build document-centric apps on relational data or create SQL apps on documents.
- Experience simplicity by retrieving and storing all the data needed for an app in a single database operation. Duality Views provide fully updateable JSON views over data. Apps can read a document, make necessary changes, and write the document back without worrying about underlying data structure, mapping, consistency, or performance tuning. 
- Enable flexibility and simplicity in building multiple apps on same data. Developers can use the power of Duality View to define multiple JSON Views across overlapping groups of tables. This flexible data modeling makes building multiple apps against the same data easy and efficient.
- Duality Views eliminate the inherent problem of data duplication and data inconsistency in document databases. Duality Views are fully ACID (atomicity, consistency, isolation, durability) transactions across multiple documents and tables. It eliminates data duplication across documents data, whereas consistency is maintained automatically. 
- Build apps that support high concurrency access and updates. Traditional locks don’t work well for modern apps. A new lock-free concurrency control provided with Duality View supports high concurrency updates. The new-lock free concurrency control also works efficiently for interactive applications since the data is not locked during human thinking time.

**_Estimated Time: 20 minutes_**

### About Product/Technology - Property Graphs on 23ai Free
In Oracle Database 23ai Free - Developer Release the GRAPH_TABLE function and MATCH clause of the new SQL:2023 standard enable you to write simple SQL queries to follow connections in data.  This workshop illustrates how you can model your data as a graph and run graph queries in SQL to quickly see relationships in your data that are difficult to identify otherwise.

**_Estimated Time: 30 minutes_**

### Objectives

About JSON-relational duality views -> This workshop aims to provide hands-on experience with JSON-relational duality views, demonstrating how to get the strengths of both JSON and relational data models. You will learn how to create, query, and update JSON-relational duality views using SQL and REST.

About Operational Property Graphs -> In this lab, you will :
* Create a PROPERTY GRAPH from relational tables
* Run graph pattern queries in SQL, using the new syntax from the SQL:2023 standard

### Prerequisites

This workhop assumes you have:
 * Oracle Database 23ai
 * Knowledge of SQL

## Learn More
* [JSON Relational Duality: The Revolutionary Convergence of Document, Object, and Relational Models](https://blogs.oracle.com/database/post/json-relational-duality-app-dev)
* [JSON Duality View documentation](http://docs.oracle.com)
* [Blog: Key benefits of JSON Relational Duality] (https://blogs.oracle.com/database/post/key-benefits-of-json-relational-duality-experience-it-today-using-oracle-database-23c-free-developer-release)
* [Oracle Property Graph](https://docs.oracle.com/en/database/oracle/property-graph/index.html)
* [SQL Property Graph syntax in Oracle Database 23ai Free - Developer Release](https://docs.oracle.com/en/database/oracle/property-graph/23.1/spgdg/sql-ddl-statements-property-graphs.html#GUID-6EEB2B99-C84E-449E-92DE-89A5BBB5C96E)

## Acknowledgements

- **Author** - Kaylien Phan, Thea Lazarova, William Masdon
- **Contributors** - Melliyal Annamalai, Jayant Sharma, Ramu Murakami Gutierrez, Rahul Tasker, David Start, Ranjan Priyadarshi
- **Last Updated By/Date** - Kaylien Phan, Thea Lazarova, Database Product Management, April 2023
