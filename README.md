# RapidData

**Introduction**

**RapidData** is an open-source, real-time, low-latency, high-throughput stream processing framework.


RapidData is a project that provides scalable, reliable, and persistent high-throughput
event processing with high-level Java APIs using Hadoop and HBase.


There are many applications that can take advantage of its features:

- Ability to handle extremely large data flows;
- Exactly-once event processing using an app-level Java API with consistency, reliability, and persistence;
- Streaming database using a SQL-like language to filter, group and join data streams in-memory;
- Runs collections of queries using pipelined query plans;
- Able to transparently handle complex record routing in large parallelized implementations;
- Runs and scales as a native Apache Hadoop YARN Application;
- Reads, writes, and tightly integrates with HDFS and HBase;
- Supports a significant amount of parallelization;
- Fault-tolerance and horizontal scalability without burdening the developer;
- Enterprise security features with debugging, logging, and monitoring tools; and
- Simpler programming model, tools and UI; and
- Open-source software and development process.


## Is It Building?

Builds                                                            
------------------------------------------------------------------         
[GitHub Version](https://github.com/gauravCodebase/rapiddata.git) 


## Getting Started

### Prerequisites

RapidData is supported on *NIX systems such as Linux and Macintosh OS X.
It is not supported on Microsoft Windows.

To install and use RapidData and its included examples, there are a few prerequisites:

  1. JDK 6 or JDK 7 (required to run RapidData; note that $JAVA_HOME should be set)
  2. GCC
  3. G++
  4. Apache Maven 3.0+ (required to build the example applications)
  
Note: To run the RapidDataSQL Stream Engine outside of RapidData, libz, Perl 5.x, and Python 3.x are required.



### Run Instructions

To run RapidData in standalone mode:

    $ run_standalone.sh <path-to-flow-jar> <flow-class-name> <run-time-args>

To run RapidData in distributed mode:

    $ run_distributed.sh <zookeeper-quorum> <hdfs-namespace>

### Building from Source

You can also build RapidData directly from the latest source code:

    git clone https://github.com/gauravCodebase/rapiddata.git
    cd rapiddata
    mvn clean package -DskipTests -Pdist


