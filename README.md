Assignment 1

1.	When RDD’s are created, the transformations performed on it are logged rather the actual data. This log of transformations is known as an RDD lineage. It can also be said that RDD lineage is a graph that shows the dependencies between transformations in spark.  

2.	Consider a cluster of 100 nodes and your application has 10 transformations. One of the nodes fails or disconnects from the cluster during the execution. For spark, this is no problem because RDD’s are fault tolerant. If there is a failure in a node, the already built RDD lineage graph will be used to reprocess that specific partition of the RDD on that node.

3.	Parallelism is controlled in spark by controlling the number of partitions that are spread across the nodes in the cluster. The more the partition, the greater and better the parallelism. 

4.	Map - This is used for transformation in spark. Map method when called, the function in it produces one output for each input element
FlatMap – This is used for transformation in spark also. FlatMap method when called upon flattens the output. For more clarification, when flatMap is called, the function in it returns a list of element (0 or more) as an iterator. 


5.	The benefits of spark architecture include:

a.	It is faster than all of its other counter-parts in processing

b.	It has RDD as its main abstraction i.e. it can re-process lost partition with linear graphs so you don’t have to spend time mirroring.

c.	It is general purpose i.e. you don’t have to learn many frameworks to run a sophisticated pipeline involving iterative, live streaming and batch processing. All is incorporated in spark. 

d.	Rich and easy to use API’s and library for languages such as SCALA, PYTHON, JAVA and R

e.	It can read files from various such as Cassandra, HDFS etc. No limitation in the sources of files it can be fed and processed. 
