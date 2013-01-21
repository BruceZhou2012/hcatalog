Apache HCatalog
===============
HCatalog is a table and storage management service for data created using Apache 
Hadoop.

The vision of HCatalog is to provide table management and storage management layers
for Apache Hadoop. This includes:

 * Providing a shared schema and data type mechanism.
 * Providing a table abstraction so that users need not be concerned with where
   or how their data is stored.
 * Providing interoperability across data processing tools such as Pig, Map
   Reduce, Streaming, and Hive. 

Data processors using Apache Hadoop have a common need for table management
services. The goal of this table management service is to track data that exists in
a Hadoop grid and present that data to users in a tabular format. HCatalog
provides a single input and output format to users so that individual users need
not be concerned with the storage formats that are chosen for particular data
sets. Data is described by a schema and shares a datatype system.

Users are free to choose the best tools for their use cases. The Hadoop project
includes Map Reduce, Streaming, Pig, and Hive, and additional tools exist such
as Cascading. Each of these tools has users who prefer it, and there are use
cases best addressed by each of these tools. Two users on the same grid who
share data are not constrained to use the same tool but with HCatalog are free
to choose the best tool for their use case.  HCatalog presents data in the same
way to all of the tools, providing interfaces to each of them.

For the latest information about HCatalog, please visit our website at:

   http://incubator.apache.org/hcatalog

and our wiki, at:

   https://cwiki.apache.org/confluence/display/HCATALOG

Getting Started
===============

```bash
$ mkdir mapr-hcatalog-0.4.0
$ cd mapr-hcatalog-0.4.0
$ git clone git://github.com/mapr/hcatalog.git .
$ git checkout branch-0.4-mapr

To build HCatalog artifacts (jars and the pom file):

$ ant package

To build and deploy HCatalog artifacts in a remote SNAPSHOT repository:

$ export MAPR_SNAPSHOTS_REPO=<URL:/path/to/snapshots/>
$ ant mvn-deploy

To generate tarball:

ant tar

The tarball is located in the build/ directory as hcatalog-0.4.1-dev.tar.gz

Using HCatalog artifacts with MapR patches in your Maven Project
================================================================

Add the following dependency to your project's pom.xml.

```xml
<dependency>
  <groupId>com.mapr.hcatalog</groupId>
  <artifactId>hcatalog</artifactId>
  <version>${mapr.hcatalog.version}</version>
</dependency>
```
