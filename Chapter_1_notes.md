# 1. Introduction to Big Data 

## What is BigData?  
A collection of data that is too big to be handled by traditional data  management tools or data processing application.
Eg. When Netflix recommend movies or shows to you that is BigData at work.  

### 5 V’s in Big Data   

| V's | Description |
| ----------- | ----------- |
| Volume | data is getting bigger and bigger  |
| Variety | different kinds of data is being generated(structured, semi, unstructured)  |
| Velocity | velocity means the speed of something in a given direction, data is being generated at an alarming rate  | 
| Value | how can we mine the useful value from the data, we have to make sure the data generated makes sense and we can get insight from it  | 
| Veracity | veracity means the accuracy and correctness of data  | 
	

### Big Data Analytics  
**Opportunities**: faster and better decision making, cost reduction, next generation products, improved services or products  
Eg. IBM Smart Meter Solution  
IBM offers an integrated suite of products designed to enable IT to leverage big data in a variety ways that can contribute to the success of energy companies.  
Solution:  
A) Data Warehousing  
B) User Data Security  
C) Data Mining  
D) Data Analysis  
E) Reporting  
	
**Problems**: Storing huge datasets, processing data with complex structure, data is growing faster than that of disk read/write speed  

<br/>


## HADOOP as a SOLUTION  

**What is Hadoop?**
Hadoop is a framework that allows us to store and process large datasets in parallel and distributed fashion.  
There are two parts of Hadoop: *HDFS* and *MapReduce*  

**A) HDFS(Hadoop Distributed File System)**  
HDFS creates a level of abstraction over the resources, from where we can see the whole HDFS as a single unit.  

HDFS has two components>> NameNode and DataNode  
NameNode: MainNode that contains metadata about the data stored  
DataNode: Data is stored in here which are commodity hardware in the distributed environment  

<img src="https://user-images.githubusercontent.com/125619716/228455864-6449ad32-2eb7-4c67-b09f-53f55dcd2543.JPG" width="400" height="280">  


### Hadoop Solving Problems
• Solving problem 1: Storing huge dataset  
<img src="https://user-images.githubusercontent.com/125619716/228455959-5f90d2a6-7df3-4a20-a5ee-b12122c620f0.JPG" width="500" height="200">  


• Solving Problem 2: Storing unstructured data  
<img src="https://user-images.githubusercontent.com/125619716/228456374-c393cea7-f83c-4026-9439-26135ed1b169.JPG" width="500" height="200">  


**B) MapReduce** 
MapReduce allows parallel processing of the data stored in HDFS  

• Solving Problem 3: Processing data faster  
<img src="https://user-images.githubusercontent.com/125619716/228456566-eaeb0c38-385b-4d08-95c7-02d3707e605c.JPG" width="500" height="280">    

*How it works?  
If the Slaves were to send the data to the Master to process at once, network congestion would happen.  
But if the Master send the processing logic to each Slaves to process locally and then only send the result back to Master, then time and resources can be saved.*  
	
<br/>

## What does a Big Data Engineer Do?   
	1. Design, Develop, Construct, Install, Test & Maintain the complete infrastructure of data management and processing systems  
	2. Build pipeline for data collection and storage, make the data consumable for Data Scientists and Data Analysts to drive insights  
	3. Build data warehouses, systems should all be scalable, robust and fault tolerant  
	4. Take care of the process of ETL(Extract, Transform and Load)  
	5. Performance tuning  


### Responsibilities  
- Data Ingestion: Acquire data from multiple sources and ingest them into data lake  
- Data Transformation: Convert data from one format to another, or from one structure to another based on use-case  
- Performance Optimization: Scalable and efficient system(optimize queries performance, denormalize partition and index data models, tools and concepts) 


<img src="https://user-images.githubusercontent.com/125619716/228457403-6362c681-c605-47b2-84f1-a89dbc177fbe.JPG" width="500" height="280">    

**1. Big Data Frameworks**  
<img src="https://user-images.githubusercontent.com/125619716/228457489-affcb230-02da-4108-922a-e11bb91c9555.JPG" width="400" height="280">   

**2. Real time processing frameworks** - Apache Spark  

**5. NoSQL Databases** - Cassandra(good for application with fast and random read and write), MongoDB(schema free DB, master/slave architecture), Apache Hbase(On top of HDFS). 

**6. Programming Languages** - Python, R, Java  

**7. ETL/Data warehousing** - data warehousing is used for analytics and reporting, Informatica, Talend(recomm to start with this if beginner), Microsoft SQL Server, QlikView   

**8. Operation Systems** - Windows, Linux, Unix  



<br/>

## What is Big Data Testing?  
Big Data Testing is the procedure that involves examining and validating the functionality of the Big Data Applications.  


**Strategies**: Batch Processing(HDFS), Real-Time Processing(Spark), Interactive Processing(Hive SQL)  


**Big Data Forms:**  
>a. Structured [data warehouses, database, ERP&CRM]  
>b. Semi-Structured [CSV, XML, JSON]  
>c. Unstructured [Audio, Video, Image]  

<br/>

### <ins>3 Phases of Big Data Testing</ins>  
**a. Data Ingestion(Tool: Talend)**  
Data is loaded from source into Big Data System. The storage might HDFS, MongoDB or others. Then the data is cross-checked for errors and missing values.  

**b. Data Processing**  
The key-value pairs for the data get generated. The MapReduce logic is applied to the nodes and checked if the algorithm works fine anot.  

**c. Data Validation**  
The output generated is ready to be migrated to data warehouse. Here, the transformation logic is checked, the data integrity is verified and the key-value pairs at the location are validated for accuracy.  
	
<br/> 


### <ins>Types of Testing Available</ins>  
**Unit Testing**  

**Functional Testing:**  
<img src="https://user-images.githubusercontent.com/125619716/228458388-efc7f63d-1c36-4f64-abc4-ccfff18cd245.JPG" width="300" height="180">  


**Non Functional Testing:**  
<img src="https://user-images.githubusercontent.com/125619716/228458438-c529360a-fe35-42dd-a86f-8708bde6c84e.JPG" width="300" height="180">  

**Performance Testing:**  
<img src="https://user-images.githubusercontent.com/125619716/228458511-1a4b8a45-8878-4b8e-9892-7b598093e07c.JPG" width="300" height="180">    
<img src="https://user-images.githubusercontent.com/125619716/228458604-8d22b293-082c-492b-b6f3-78370430e551.JPG" width="300" height="180">    


**Architecture Testing:**  
This test concentrates on establishing a stable Hadoop architecture.  
The architecture of Big Data Processing Application plays a key role in achieving smooth operation.  
Poor architecture leads to >>  
<img src="https://user-images.githubusercontent.com/125619716/228463844-d3212c88-1561-423d-847b-e1bf9e859564.JPG" width="300" height="180">    

<br/>  

### <ins>Big Data Testing Tools</ins>  
Data Ingestion - ZooKeeper, Kafka, Sqoop  
Data Processing - MapR, Hive, Apache Pig  
Data Storage - Amazon S3, HDFS  
Data Migration - Talend, CloverDX  

<br/>  

### Difference between Big Data Testing and Traditional Testing  
	1. Big Data Testing supports all types of data testing while tradi testing only supports structured data testing.  
	2. Big Data Testing requires R&D while tradi testing does not.  
	3. Data size is unlimited in BD testing while is limited in tradi testing.  
	4. BD testing requires special environment while tradi does not.  

