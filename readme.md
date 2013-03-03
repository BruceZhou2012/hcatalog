Apache HCatalog
===============

HCatalog is a table and storage management service for data created using Apache 
Hadoop.

HCatalog provides table management and storage management layers for Apache Hadoop.
This includes:

 * Providing a shared schema and data type mechanism.
 * Providing a table abstraction so that users need not be concerned with where
   or how their data is stored.
 * Providing interoperability across data processing tools such as Pig, Map
   Reduce, Streaming, and Hive. 

Data processors using Apache Hadoop have a common need for table management
services. The goal of this table management service is to track data that exists in
a Hadoop grid and present that data to users in a tabular format. HCatalog
provides a single input and output format to users, irrespective of storage formats for specific data sets. Data is described by a schema and shares a datatype system.

Users are free to choose the best tools for their use cases. The Hadoop project
includes MapReduce, Streaming, Pig, and Hive. Additional tools such
as Cascading are available. Each of these tools has users who prefer it, and there are use cases best addressed by each of these tools. Two users on the same grid who
share data are not constrained to use the same tool. With HCatalog, each user can choose the best tool for their use case.  HCatalog presents data in the same
way to all of the tools, providing interfaces to each of them.

For the latest information about HCatalog, please visit our [website](http://incubator.apache.org/hcatalog) or [wiki](https://cwiki.apache.org/confluence/display/HCATALOG).