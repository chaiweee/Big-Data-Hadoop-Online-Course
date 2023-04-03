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


