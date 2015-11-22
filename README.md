# analyticsClass
Materials for the Analytics Class

# Instructions

Clone this repository to the VM - The Cloudera VM has Git
   - Follow the Git Hub Instructions on cloning a repository

On the Cloudera VM

hdfs dfs -mkdir /home/cloudera/analytics
hdfs dfs -mkdir /home/cloudera/document

unzip the analytics demo first
hdfs dfs -put part-m-00000 /home/cloudera/analytics/

Remove the part-m-00000 file

unzip the document file
hdfs dfs -put part-m-00000 /home/cloudera/document/

hbase org.apache/hadoop.hbase.mapreduce.Import analytics_demo /home/cloudera/analytics

hbase org.apache/hadoop.hbase.mapreduce.Import analytics_demo /home/cloudera/document




