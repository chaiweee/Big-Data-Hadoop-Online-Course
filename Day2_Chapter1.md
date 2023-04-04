### Big Data in Real World

**Clinical Analytics**  

<img width="300" alt="Screenshot 2023-03-30 at 8 40 03 AM" src="https://user-images.githubusercontent.com/125619716/228692047-d68b6129-7310-4711-8aec-902acb5c53b1.png">  

**Education**  
<img width="300" alt="Screenshot 2023-03-30 at 8 45 09 AM" src="https://user-images.githubusercontent.com/125619716/228692265-878ea108-6864-4ae9-8ee9-8aef1291ef97.png">  

**E-commerce**  
<img width="300" alt="Screenshot 2023-03-30 at 8 50 56 AM" src="https://user-images.githubusercontent.com/125619716/228693343-654f1908-2fd8-4690-8580-47362f73425d.png">  

<img width="300" alt="Screenshot 2023-03-30 at 8 55 14 AM" src="https://user-images.githubusercontent.com/125619716/228693823-82b02560-9a3b-4818-b898-6d45366b385e.png">  

Workflow  
User data is collected from various sources. That includes customer information, purchase history, reviews.  
Then we have Input Selection Module to remove noise from the data. It has single value decomposition which is used to speed up the recommendations with very fast online performance. It also has dimensionality reduction to remove a number of random variables under consideration that are not required in the data.

Then the noise free data is then fed as an input to HDFS Input in Hadoop System to undergo MapReduce to produce HDFS Output. 

The data is now ready for Data Analytics for forecasting demand and sales generation.

**Government**  
<img width="300" src="https://user-images.githubusercontent.com/125619716/228696640-1835a13a-83be-4aaa-b587-7b079310ffb0.png">  

<img width="300" src="https://user-images.githubusercontent.com/125619716/228696676-ec617faa-d996-4c1c-860e-5d730f5bc5d0.png">  

Workflow:  
Citizens or enterprise send a request through the portal.  
The requests are then send to Big Data infrastructure to be processed.  
The infrastructure has database that is not centralized, it integrates with database of different Ministries and local authorities.
Then both the databases are deployed to cloud infrastructure(to reduce the cost of storage).  
Hadoop framework is here to process the data. We run Pig and Hive queries on Hadoop data platform and then store data in HDFS and response is sent back.  


**IOT**  
<img width="300" src="https://user-images.githubusercontent.com/125619716/229698030-267412c8-b5d5-4a18-84c6-10cfc4752461.png">  
<img width="300" src="https://user-images.githubusercontent.com/125619716/229698038-b6b715f6-dd56-430e-9503-a0855915af04.png">  

Amsterdam city is implementing Smart City Concept.


**Media & Entertainment**   

<img width="300" src="https://user-images.githubusercontent.com/125619716/229698099-7b0dea2a-3cc0-45f2-af79-807cc78f66f1.png">  
<img width="300" src="https://user-images.githubusercontent.com/125619716/229698107-77e1dc4c-3615-4b98-96f8-f92733b58fba.png">  


Netflix has ton of users in its database. They process and analyze the data to discover pattern in the data.  
Then Netflix has a new user request. The new user then search through Netflix search engine.  
Based on the user choice, Netflix rank videos and provide them with customized experience.  
User continues to watch and Netflix provides Video Similarity Algorithm.  

How is the video ranking done?    
<img width="300" src="https://user-images.githubusercontent.com/125619716/229698155-37bd0e36-a9f3-4c4c-af95-78ee7e0fdb50.png">  
  
Netflix uses NoSQL Cassandra because it is highly scalable and strong on performance.  
Priam is a Cassandra helper tool and also a Netflix cluster management tool that simplifies Netflix Administration.  
The query data is stored in S3-SS Tables in table format.  
Aegisthus is a platform built by Netflix engineers to work on MapReduce. It helps to convert the Cassandra S3-SS tables into queryable format.  
S3-json is a JavaScript object notation that is used to structure query data.  
Based on all the above the decision is made and the video ranking is given to user.  


### Why do we need Big Data Analytics?  
	1. Making smarter and more efficient organizations  
	2. Optimize business operations by analyzing customer behaviour  
	3. Cost reduction  
	4. Next Generation Products - smart yoga mat??  

**Stages in Big Data Analytics**  
	1. Identifying the problem  
	2. Designing data requirement  
	3. Preprocessing data  
	4. Performing analytics over data  
	5. Data visualization  



|   | Type of Big data Analytics |	Description |
| - | -------------------------- | ------------ |
|1	| Descriptive Analysis	     | <img width="300" src="https://user-images.githubusercontent.com/125619716/229698851-67baa545-547d-4d09-9f8e-1e1acfebce00.png">   Example: Netflix is using to find correlations between different movies the user is watching to improve their recommendation engine.  |
|2	| Predictive Analysis	       | <img width="300" src="https://user-images.githubusercontent.com/125619716/229698887-e59c81a8-b400-4910-b61f-2e5688904eec.png"> |
|3  | Prescriptive Analysis	     | <img width="300" src="https://user-images.githubusercontent.com/125619716/229698972-06ad4805-bb85-4357-b70d-d466c633b8d8.png">   This analysis uses optimization and simulation algorithms to advise on the possible outcomes and answer the question of we should we do.  It allows user to prescribe a few different possible actions and then guide them towards the solution. Involves ML, model, rules and so to advise action.  |
|4  |	Diagnostic Analytics	     | <img width="300" src="https://user-images.githubusercontent.com/125619716/229699083-07cd0ebf-b636-4e84-bb74-b0e8961955f3.png"> |

<img width="300" src="https://user-images.githubusercontent.com/125619716/229699370-6da396fd-ad37-4d0f-a48f-1254d4bb0e79.png">   

<img width="300" src="https://user-images.githubusercontent.com/125619716/229699410-330d1a6e-a16e-4243-885e-0bdacdce114b.png">
Starbucks gather user information through point system.   

</br>

<img width="300" src="https://user-images.githubusercontent.com/125619716/229699433-8546fa9a-072b-42a3-9ec4-aadd5931a98a.png">  
They observe the baskets of customer and will arrange the location of product with high similarity together.  


</br>

