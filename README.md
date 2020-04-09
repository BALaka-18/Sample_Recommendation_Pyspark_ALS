# Sample_Recommendation_Pyspark_ALS
A sample notebook that illustrates Apache Spark's ALS recommendation algorithm. 
___________________________________________________________________________________________________________________________________________

### Installing Spark, Hadoop and Java into Colab

1. Copy and Paste this :

!apt-get install openjdk-8-jdk-headless -qq > /dev/null

!wget -q http://mirrors.viethosting.com/apache/spark/spark-2.4.5/spark-2.4.5-bin-hadoop2.7.tgz

!tar xf spark-2.4.5-bin-hadoop2.7.tgz  -----> Make sure you're using the latest version of Spark.

!pip install -q findspark

If you get an error in the 3rd line, make sure you have mentioned the latest version of Spark. Otherwise, it won't work.
Check the latest Spark version : 
https://downloads.apache.org/spark/

2. Copy and Paste this :

import os

os.environ["JAVA_HOME"] = "/usr/lib/jvm/java-8-openjdk-amd64"

os.environ["SPARK_HOME"] = "/content/spark-2.4.5-bin-hadoop2.7"

3. Then initialize before using :

import findspark

findspark.init()

_______________________________________________________________________________________________________________________________________

##### Now you've set up your spark environment. Initialize a session to start working.


