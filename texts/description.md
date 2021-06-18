# Redis Cluster
 
**What is it**

This repository will provide you with the option to deploy a fully functional Redis Cluster

**Deployment**
In order to get this solution instantly deployed, click the "Deploy to Jelastic" button

[![GET IT HOSTED](https://raw.githubusercontent.com/jelastic-jps/jpswiki/master/images/getithosted.png)](https://app.j.layershift.co.uk/?manifest=https://raw.githubusercontent.com/layershift/jps_redis_cluster/main/redis_cluster.jps)

To deploy this package to Jelastic Private Cloud, import [this JPS manifest](https://raw.githubusercontent.com/layershift/jps_redis_cluster/main/redis_cluster.jps) within your dashboard ([detailed instruction](https://docs.jelastic.com/environment-export-import#import)).

For more information on what Jelastic add-on is and how to apply it, follow the [Jelastic Add-ons](https://github.com/jelastic-jps/jpswiki/wiki/Jelastic-Addons) reference.

**Instalation**

On the first screen of the instalation you will find the option to select the number of cloudlets you want to assign to the nodes (at least 10 is recommended), the Environment name and display name, and the Region where you want to deploy.
![Install](https://raw.githubusercontent.com/layershift/jps_redis_cluster/main/images/deploy.PNG)

The cluster will be deployed with 3 Master nodes and 3 Slave nodes. The nodes will be deployed on different hardware Servers in sets of three, as follows:
Master node1: Hardware node A
Master node2: Hardware node B
Master node3: Hardware node C
Slave node1: Hardware node A
Slave node2: Hardware node B
Slave node3: Hardware node C


