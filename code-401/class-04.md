# Reading Notes 4

This topic is important because data modeling helps understand tables/databases when they get more complicated. It's also important to be able to know the best kind of database for what you want to build.

## nosql vs sql

1. What type of database is the best fit for the complex query intensive environment?

    Complex queries are a good fit for a SQL database.

2. What type of database is the best fit for hierarchical data storage?

    NoSQL databases are better for hierarchical data storage.

3. Describe the differences in scalability between a SQl and NoSQL database as though you were speaking to a non-technical friend.

    SQL databases are vertically scalable which means they increase their power by strengthening the resources that they already have. For example, if you want to serve more food to people, you increase the size of the plates.

    NoSQL databases are horizontally scalable which means they increase their power by adding more resources. For example, if you want to serve more food to people, you increase the amount of plates.

Resource: <https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool>

## sql modeling techniques

1. Among data tables, what is a one-to-many relationship, and how do we “relate” them?

    A one-to-many relationship is when an entry in one table is related to multiple entries in another. We relate them with a primary key and foreign key. Both those keys are columns with IDs.

2. Prior to designing your relational database, it might be useful to ___ a ___ of the database tables and their relationships.

    Draw a diagram.

3. Explain the difference between a primary and foreign key.

    A primary key uniquely identifies each entry in a table. A foreign key has values that match primary key values in the other table. There can be multiple of the same foreign key values in a table, while primary key values in a table are all unique.

Sources: <https://www.essentialsql.com/get-ready-to-learn-sql-7-simplified-data-modeling/> and ChatGPT.

## sql vs nosql (video)

1. How do we treat keywords and parameters differently in SQL syntax?

    Keywords are in all caps. Parameters are in parenthesis and either have colons or @ signs in front of them.

    Source: ChatGPT

2. Define normalization within the context of schemas and data.

    Normalization is dividing large tables into smaller ones that all have relations with each other. It organizes the data more efficiently.

    Source: ChatGPT

3. Explain the difference between one-to-one, one-to-many, and many-to-many relationships to a non-technical recruiter.

    - __One-to-one__: One entry in one table links to another entry in another table (like a ‘contact_id’ from one table linking to an ‘id’ in another. Both have no duplicates). Example: Every User (table) has one Contact (table), and vice versa.

    - __One-to-many__: When an entry in one table is related to multiple entries in another. Example: One User (table) has multiple Contacts (table) linked to them.

    - __Many-to-many__: When both tables have entries that are assigned to multiple entries in the other table. It requires an extra table to connect everything. Example: Users (table) can have multiple Roles (table) and a Role can belong to multiple Users.

    Source: <https://www.youtube.com/watch?v=ZS_kXvOeQ5Y>

## Reflection

My learning goals are to learn more about how to use different kinds of databases and make collections. And to be able to do everything in the lab assignment.

## Things I want to know more about
