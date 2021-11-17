# jps_redis_cluster

This repository provides an add-on to install and configure 

**Type of nodes this add-on can be applied to:**

- Standalone Redis Cluster
- Existing Compute nodes

### What can it be used for?

Redis Cluster provides a way to run a Redis installation where data is automatically sharded across multiple Redis nodes.

Redis Cluster also provides some degree of availability during partitions, that is in practical terms the ability to continue the operations when some nodes fail or are not able to communicate. However the cluster stops to operate in the event of larger failures (for example when the majority of masters are unavailable).

### So in practical terms, what do you get with Redis Cluster?

- The ability to automatically split your dataset among multiple nodes.
- The ability to continue operations when a subset of the nodes are experiencing failures or are unable to communicate with the rest of the cluster.


### Installing

[![GET IT HOSTED](https://raw.githubusercontent.com/jelastic-jps/jpswiki/master/images/getithosted.png)](https://app.j.layershift.co.uk/?manifest=https://github.com/layershift/jps_redis_cluster/blob/main/redis_cluster.jps)


During installation you are asked to select if you would like to create a new environment for the Redis cluster, or configure it on an existing environemnt (if selecting an existing evironment, please make sure there are no redis nodes already added):
![alt text](https://github.com/layershift/jps_redis_cluster/blob/main/images/starting_page.PNG)


Once the add-on is installed, it will create 6 Redis nodes, and configure them into a cluster.
All the needed information regarding conectivity is displayed on the screen, and also emailed to you!
![alt text](https://github.com/layershift/jps_redis_cluster/blob/main/images/info.PNG)


### Redis Cluster 
The Redis Cluster add-on can be found in the add-ons tab of the environment
![alt text](https://github.com/layershift/jps_redis_cluster/blob/main/images/cluster-addon.PNG)

The available options are described below:
![alt text](https://github.com/layershift/jps_redis_cluster/blob/main/images/cluster-options.PNG)
-   Show Cluster Password -> Will liste the current Redis Cluster password
-   Change Cluster Password -> Will reset the existing Cluster password (This will also provide you with all the new details needed to connect to the cluster)
-   Install Cluster Tools -> Install the Redis Cluster Tools add-on
-   Rebuild Cluster -> Will wipe all the existing data from the cluster, and reconfigure it from start
### Redis Cluster Tools

The redis cluster tools add-on can be found in the add-ons tab of the environment
![alt text](https://github.com/layershift/jps_redis_cluster/blob/main/images/add-ons.PNG)

The options available here are described bellow:
![alt text](https://github.com/layershift/jps_redis_cluster/blob/main/images/cluster-tools.PNG)

-   p3x-redis-ui -> Will open a new tab and allow you to connect to the P3X Redis Cluster User Interface
-   Show Cluster Nodes -> Will show you all the available cluster nodes, pointing out the role they have in the cluster (master/slave)
-   Show Connection Information -> Will show you the required information (including password for the cluster) to connect your application to the redis cluster
-   Ping Cluster Nodes -> Will initiate a PING command to all the nodes. The ones that are available will send a PONG reply
-   Update-p3x-redis-UI -> Will check for latest updateds for the P3X Redis Cluster User Interface and install them if available

