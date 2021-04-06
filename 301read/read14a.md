# read-14a

### Database Normalization
Database normalization is a process used to organize a database into tables and columns. The idea is that a table should be about a specific topic and that only those columns which support that topic are included.

By limiting a table to one purpose, you reduce the number of duplicate data that is contained within your database, which helps eliminate some issues stemming from database modifications.

### Reasons for Normalization
* The first is to minimize duplicate data
* the second is to minimize or avoid data modification issues
* the third is to simplify queries.

### Data Duplication and Modification Anomalies
There are three modification anomalies that can occur:
1. Insert Anomaly: There are facts we cannot record until we know information for the entire row.
1. Update Anomaly: The same information is recorded in multiple rows.
1. Deletion Anomaly: eletion of a row can cause more than one set of facts to be removed.

### Definition of Normalization
* First Normal Form – The information is stored in a relational table and each column contains atomic values, and there are not repeating groups of columns.
* Second Normal Form – The table is in first normal form and all the columns depend on the table’s primary key.
* Third Normal Form – The table is in second normal form and all of its columns are not transitively dependent on the primary key.