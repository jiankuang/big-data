# Hadoop 
IBM Hadoop course

## Architecture
cluster -> rack -> node

## HDFS
* Not POSIX compliant
* File blocks: default 64MB, recommend 128MB

### HDFS Command
`hdfs dfs -ls`

#### POSIX-like commands
cat, chgrp, chmod, chown, cp, du, ls, mkdir, mv, rm, stat, tail

#### HDFS - specific commands
* copyFromLocal / put, copyToLocal / get 
* getMerge: gets all files and merges and sorts them to only one file on local filesystem
* setRep: sets the replication factor of a file (files)

## MapReduce
* only one namenode per cluster
* only one JobTracker per cluster

## Hadoop 2.2 Architecture (YARN)

## Moving Data into Hadoop
* Data at rest: use `cp`, `copyFromLocal` or `put` commands
* Data in motion
* Data from a web server
* Data from a data warehouse

### Data Click for BigInsights
* First **Data Click Authors** create and configure offload activites
* Afterward **Data Click Users** can run these offload activities

## Java API
### I/O
#### Codec
`CompressionCodecFactory` provides a way of mapping a filename extension to a `CompressionCodec` using its `getCodec()` method