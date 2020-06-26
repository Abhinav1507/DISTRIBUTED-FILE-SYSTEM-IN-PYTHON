# DISTRIBUTED-FILE-SYSTEM-IN-PYTHON

The project aims at providing a distributed file system that is scalable, transparent and location 
independent. Simple distributed file system like HDFS (and of-course GFS). It consists of one Master 
(NameNode) and multiple Minions (DataNode). And a client for interation. It will dump metadata/
namespace when given SIGINT and reload it when fired up next time. Replicate data the way HDFS 
does. It will send data to one minion and that minion will send it to next one and so on. Reading done 
in similar manner. Will contact fitst minion for block, if fails then second and so on. Uses RPyC for 
RPC. We also take into account the fact that, nowadays the PCs, are equipped with enormously large 
hard disks. The distributed file provides the means of utilizing the hard disks of various machines in 
place. There is no need of dedicated servers. In an environment like educational institutions, lots of 
workstations with large disk space are available. So the distributed file system comprises of files that 
are stored on the hard disks of participating workstations across an interconnected network. We use a 
distributed look up mechanism to provide location independence. The distributed nature of look ups 
prevents the look up module from becoming bottleneck.

 the distributed file system 
supports the following:
1. Remote information sharing 
Thus any node, irrespective of the physical location of the file, can access the file. So, 
any system situated at any part of world is going to access the files directly by itself. 
2. User mobility 
User should be permitted to work on different nodes. So, the users are able to do work 
on any of the systems that is part of Distributed File System. 
3. Availability
For better fault-tolerance, files should be available for use even in the event of 
temporary failure of one or more nodes of the system. Thus the system should maintain 
multiple copies of the files, the existence of which should be transparent to the user.
4. Diskless workstations
A distributed file system, with its transparent remote-file accessing capability, allows 
the use of diskless workstations in a system. As a result, it reduces the cost and regular 
updating of any external storage that could have been used for storage.
