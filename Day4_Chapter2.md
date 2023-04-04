*Before 3:28:00 there were two different Spark project showing how to do analyzing and visualization with US Election data and Uber data.  
I have to skip this part first because I still havent learn how to use hadoop and spark.* 


## What is Hadoop Cluster?  
Cluster means a collection.  
A Hadoop cluster is a set of connected commodity computers. They work together so that in many respects and viewed as a single system.  
Hadoop clusters have each node set to perform the same task, controlled and scheduled by the Master.  

Advantages of Hadoop Cluster  
- Scalable - Compared to rdbms, hadoop storage network can be added only needs to add commodity hardware  
- Cost effective  
- Flexible - Can process any type of structure of data  
- Fast - Can process petabytes of data in seconds, because of the efficient data mapping capabilities  
- Resilient to failure - It is practically impossible to loss any data in a hadoop cluster as it follows data replication which acts as a backup storage unit in case of node failure  
	
	
### Hadoop Cluster Architecture  

<img width="600" src="https://user-images.githubusercontent.com/125619716/229703885-fccdd637-7250-4aae-b50b-b6935a191786.png">  


**1. HDFS - consists of NameNode, Secondary NameNode, DataNode**   
<img width="600" src="https://user-images.githubusercontent.com/125619716/229704020-3b05bbc6-cfda-4ae5-a519-87b8963f3a5b.png">  
<img width="600" src="https://user-images.githubusercontent.com/125619716/229704036-86b94ab9-1b56-45e9-a3b8-2372554bbd3c.png">  

NameNode does:   
- Designed to store the metada of the actual data   
- First one to encounter the clients requests for data  
- Then transfer the request to DataNode which store the actual data  
- Manage health of all DataNodes  
- It receives heartbeat and task status from DataNode  
- If it fails to receive heartbeat from DataNode, then it consider the DataNode dead and assign the task to next one  

DataNode does:  
- Update task status and health status to NameNode in the form of heartbeat  

Secondary NameNode does:  
- Not actually a backup of NameNode  
- Acts as a buffer which saves the latest updats to the FS-image which are obtained in the intermediate process and updates them to the final FS-image  


**2. YARN - consists of Node Manager, App Master, container**  
<img width="600" src="https://user-images.githubusercontent.com/125619716/229704542-c4997de0-9870-4cff-9ca5-f7d5c9d263ba.png">  

Node Manager does:  
- A java utility that runs as a separate process from weblogic server
- Allows you to perform common operations for a managed server regardless of its location with respect to the administration server

App Master does:  
- Negotiating the resources between Resource Manager and Node Manager

Container does:  
- A collection of reserved amount of resources allocated from the Resource Manager to work with the task assigned by the Node Manager

</br>

### Overview of Hadoop Cluster which consists of Racks  
<img width="600" src="https://user-images.githubusercontent.com/125619716/229704698-34c47720-d1c7-41d7-9840-1594e1402bd5.png">  

**Rack Awareness Algorithm**  
- It is all about data storage  
- Reduces latency as well as provide fault tolerance by replicating data block  
- It says that the first replica of a block will be stored on a local rack & the next two replicas will be stored on a different (remote)rack  
<img width="600" src="https://user-images.githubusercontent.com/125619716/229704785-9225c68d-488b-470c-bb88-ba858e13c867.png">  

*The block 1 in rack-1 datanode1 is stored in rack-2 DN6 and DN8, The block 3 in rack-3 DN11 is stored in rack-1 DN2 and DN4*  

</br>

*From 3:37:51 onwards, the video begins a practical session to build a hadoop cluster with a Master and 2 Slaves using VM.  
Since I don’t have any basics on Hadoop, I had to begin with installing Hadoop on my Mac to understand.  
The article I refer to is: https://towardsdatascience.com/installing-hadoop-on-a-mac-ec01c67b003c    
Another useful site: https://ashwin.cloud/blog/single-node-cluster-mac/  
This article shows how to install single node hadoop cluster.*  
*The video shows how to install Hadoop on Windows at 4:04:00*  

</br>

Hadoop is both a command line interface as well as an API.    
It does not require any tool in specific to manage and monitor utilities.  
There are some options available such as:  
1. HortonWorks  
2. Ambari - most popular  
<img width="600" src="https://user-images.githubusercontent.com/125619716/229705106-0a7c5976-72b7-45d3-9c5e-eee6773e5356.png">  
<img width="600" src="https://user-images.githubusercontent.com/125619716/229705117-efd92bf3-976a-4e54-a592-8777394727b8.png">  


### Factors Deciding Hadoop Cluster  
| Factors | Description |
| --------------- | -------------- |
| Volume of data  | It is important for Hadoop Admin to know the volume of data he needs to deal with and accordingly plan, organize and set up the Hadoop Cluster with appropriate number of nodes for an Efficient Data Management.  |
| Data Retention  | Data Retention is a process where the user gets to remove outdated, invalid and unnecessary data from the Hadoop Storage to save space and improve cluster computation speed.  |
| Data Storage  | The obtained data is encrypted and compressed using various Data Encryption and Data Compression algorithms  so that the data security is achieved, and the space consumed to save the data is as minimal as possible.  |
| Type of Workloads  | This factor is purely performance-oriented. All this factor deals with is the performance of the cluster. The workload on the processor can be classified into three types: Intensive, Normal and Low.  |

	
### Hardware Requirement  
For the Masters:  
<img width="600" src="https://user-images.githubusercontent.com/125619716/229705771-0cae2f41-78da-4b86-9b40-4fe797c2e22d.png">  

For the Slaves(data nodes):  
<img width="600" src="https://user-images.githubusercontent.com/125619716/229705862-5a47745d-2325-4d61-b9dd-dbda277ef908.png">  


### How to plan for Hadoop Cluster?  
1. Hadoop Storage
<img width="600" src="https://user-images.githubusercontent.com/125619716/229705961-ecfe0a3b-cd11-48e8-a815-0a83c7b3e7fb.png">  
Eg.  
<img width="600" src="https://user-images.githubusercontent.com/125619716/229706071-cf99d5d0-a223-401b-9703-6839b03315bc.png">  

2. Number of Nodes  
After getting the 4S, we can estimate the number of data nodes needed.  
<img width="600" src="https://user-images.githubusercontent.com/125619716/229706116-2379f562-b027-4ff3-bc6a-329fa4979839.png">  

*D = the disk space available for each node*
In this example, we assume that 25 TB is the available disk space for single node and the initial data to be 5000 TB.   
Hence we need 200 DataNodes.   
	
	
