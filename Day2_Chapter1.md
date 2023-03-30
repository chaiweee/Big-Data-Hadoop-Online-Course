## Big Data in Real World

**Clinical Analytics**  

<img width="400" alt="Screenshot 2023-03-30 at 8 40 03 AM" src="https://user-images.githubusercontent.com/125619716/228692047-d68b6129-7310-4711-8aec-902acb5c53b1.png">  

**Education**
<img width="400" alt="Screenshot 2023-03-30 at 8 45 09 AM" src="https://user-images.githubusercontent.com/125619716/228692265-878ea108-6864-4ae9-8ee9-8aef1291ef97.png">  

**E-commerce**  
<img width="400" alt="Screenshot 2023-03-30 at 8 50 56 AM" src="https://user-images.githubusercontent.com/125619716/228693343-654f1908-2fd8-4690-8580-47362f73425d.png">  

<img width="400" alt="Screenshot 2023-03-30 at 8 55 14 AM" src="https://user-images.githubusercontent.com/125619716/228693823-82b02560-9a3b-4818-b898-6d45366b385e.png">  

User data is collected from various sources. That includes customer information, purchase history, reviews.  
Then we have Input 

**IOT**  
<img width="400" src="https://user-images.githubusercontent.com/125619716/228775652-51fea9f2-c202-4b75-b65b-6e20b1636af2.png">   
<img width="400" src="https://user-images.githubusercontent.com/125619716/228775807-79ec763c-e411-4525-b7c4-53161fa03cdf.png">  

Amsterdam city is implementing Smart City Concept.  


**Media & Entertainment**  

<img width="400" src="https://user-images.githubusercontent.com/125619716/228776005-445c309f-1c28-416a-a44e-ae4f7290e8c8.png">  
<img width="400" src="https://user-images.githubusercontent.com/125619716/228776038-530f79d2-3ee9-43de-80b6-144625699a04.png">  

Netflix has ton of users in its database. They process and analyze the data to discover pattern in the data.  
Then Netflix has a new user request. The new user then search through Netflix search engine.  
Based on the user choice, Netflix rank videos and provide them with customized experience.  
User continues to watch and Netflix provides Video Similarity Algorithm.  

How is the video ranking done?  

<img width="400" src="https://user-images.githubusercontent.com/125619716/228776318-683cb105-a53a-4c51-9168-b35532e4d1c9.png">

Netflix uses NoSQL Cassandra because it is highly scalable and strong on performance.
Priam is a Cassandra helper tool and also a Netflix cluster management tool that simplifies Netflix Administration.
The query data is stored in S3-SS Tables in table format.
Aegisthus is a platform built by Netflix engineers to work on MapReduce. It helps to convert the Cassandra S3-SS tables into queryable format.
S3-json is a JavaScript object notation that is used to structure query data.
Based on all the above the decision is made and the video ranking is given to user.

</br>

## Why do we need Big Data Analytics?  
	1. Making smarter and more efficient organizations  
	2. Optimize business operations by analyzing customer behaviour  
	3. Cost reduction  
	4. Next Generation Products - smart yoga mat??  

**Stages in Big Data Analytics**  
Identifying the problem  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;↓  
Designing data requirement  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;↓   
Preprocessing data  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;↓  
Performing analytics over data  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;↓  
Data visualisation  

</br>

| Type of Big Data Analytics | Description |
| ----------- | ----------- |
| Descriptive Analysis | <img width="400" src="https://user-images.githubusercontent.com/125619716/228777584-8010d6b6-b57f-4493-8ed3-c43fec4cfcd0.png">  </br>  Example: Netflix is using to find correlations between different movies the user is watching to improve their recommendation engine.|
| Predictive Analysis | <img width="400" src="https://user-images.githubusercontent.com/125619716/228778014-b0cc2696-fe1b-47c7-a1e9-b981a6dbda05.png"> |
| Prescriptive Analysis | <img width="400" src="https://user-images.githubusercontent.com/125619716/228778043-ae2a8768-fcc5-4a92-b15a-1483548c44b7.png"></br>   This analysis uses optimization and simulation algorithms to advise on the possible outcomes and answer the question of we should we do. It allows user to prescribe a few different possible actions and then guide them towards the solution. Involves ML, model, rules and so to advise action.  | 
| Diagnostic Analytics | <img width="400" src="https://user-images.githubusercontent.com/125619716/228778183-4bf8f11e-7dfc-4457-b23d-4bc36230b3b6.png"> |

</br>

<img width="400" src="https://user-images.githubusercontent.com/125619716/228778768-22e32459-3b1a-446b-86dc-947cdb74378d.png">  

<img width="400" src="https://user-images.githubusercontent.com/125619716/228778860-2c0d26f9-a6d0-4ba5-9f28-d19e810de852.png">  
	Starbucks gather user information through point system. 
  
<img width="400" src="https://user-images.githubusercontent.com/125619716/228778946-01028df4-c05b-4cae-bf4f-9da5f87a2091.png">  
	They observe the baskets of customer and will arrange the location of product with high similarity together.  

</br>

## Introduction to Hadoop and Spark  

<img width="400" src="https://user-images.githubusercontent.com/125619716/228779108-98dffefb-76f3-4dc2-9cc0-6eeacb3d03f1.png">  

<img width="400" src="https://user-images.githubusercontent.com/125619716/228779085-0ca5da65-18c4-48a4-acb1-e1bf165eca43.png">  


By using Spark and Hadoop together,  
1. Spark processes data 100 times faster than MapReduce(Faster Analytics)  
2. Spark Applications can run on YARN leveraging Hadoop cluster(cost optimization)  
3. Apache Spark can use HDFS as its storage (avoid duplication)    


<img width="400" src="https://user-images.githubusercontent.com/125619716/228779414-99583d21-31ce-4d22-806d-c5bbcddc6cd5.png">  

</br>

### Spark  

Spark Core Components:  
<img width="400" src="https://user-images.githubusercontent.com/125619716/228779520-0e8908d9-936d-495b-bdfe-766a91da0777.png">  


- Spark Core Engine  
This is the base engine for large scale parallel and distributed data processing.  
It is responsible for:  
  * memory management and fault recovery  
  * Scheduling, dustributing and monitoring jobs on clusters  
  * Interacting with storage systems  
                      
                      
<img width="400" src="https://user-images.githubusercontent.com/125619716/228779686-f3e8be20-b3b8-401a-892e-081e457e953b.png">  


- Spark SQL  
	Spark SQL integrates relational processing with Spark's functional programming It also provides support for various data sources and makes it possible to weave SQL queries with code transformations.  
	
<img width="400" src="https://user-images.githubusercontent.com/125619716/228779725-4771d756-b6bb-4122-955b-6d77429a0540.png">  

*Data Frame API is the distributive collection of data that is organized into named columns that is similar to relational tables in SQL that is used to store data.*  
	
- Spark Streaming  
- MLlib  
- GraphX  
- SparkR  



