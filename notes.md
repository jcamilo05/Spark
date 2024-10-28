# Spark's Notes:

**HDFS:** Hadoop data file system - allow us to form a cluster of computers and used the combined capacity to storing our data. 

**Map Reduce** Allow us to use the combined computing power of the cluster and use it to produce the enormous data volume that we stored in HDFS. 

The previous is a huge advantage because we don´t have to use a large and expensive super computers to store and process large amount of data. Instead hadoo allows to combined regular computers into a cluster and create the storage and computation needed.

## Data lake
Like Data warehouse we collect data from different sources and stored them in HDFS, then we used the map reduced and spark to process the data and prepare new data models to generating reports and business insights.

![datalake](./img/datalakehouse.png)

Data lake allow us to collect and process huge volumes of semi-structure and unstructured data.

The two major problems with data lakes that couldn't support properly was **Transaction and consistency** and **reporting performance**, the it becomes to adopt a different architecture for implementing data lakes.
The first one they start to integrate relational databases and data warehouse for reporting and BI purposes (second images's column).
The approach basically is it collect the data in data lake storage and is processed using apache Spark and stored the result in a Data warehouse, finally is make the connection between the BI and reporting, machine learning still work on the data lake, but BI and reporting again shifted to the data warehouse.

Data storage management that is data lake basically are done in Cloud Object stores such as Amazon S3, Azure Blob, Azure Data lake storage or Google cloud storage.

**Data processing and transformation**: This is basically done with the following steps

1. Initial data quality check
2. Transforming and preparing data
3. Correlating, aggregating, Analysing and extracting business insights.
4. Applying machine learning model.

The previous steps are made with Apache Spark  

## What is Apache Spark?

Is a distributed data processing framework, this framework provides an interface for programming clusters with implicit data parallelism.

Apache Sparks can run in two kind of environments, in the cloud platforms and on site platform (local machine).

