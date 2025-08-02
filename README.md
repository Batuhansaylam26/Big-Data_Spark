# Install Scala on your computer

Firstly, The scala language is installed on the computer via following bash code block.</br>

```bash
curl -fL https://github.com/coursier/coursier/releases/latest/download/cs-x86_64-pc-linux.gz | gzip -d > cs && chmod +x cs && ./cs setup
```

After the installing, the computer is rebooted.</br>

Then check the scala.</br>

```bash
scala -version
```

Output:</br>
```bash
Scala code runner version: 1.8.4
Scala version (default): 3.7.2

```

After all, the scala and the compiler of scala can be launched via </br>

```bash
cs launch scala:3.7.2

cs launch scalac:3.7.2

```

# [Print "Hello World"](./hello.scala)

Firstly, the "Hello world" is printed on the screen.</br>
```bash
scala run hello.scala
```
Output:</br>
```bash
Starting compilation server
Compiling project (Scala 3.7.2, JVM (21))
Compiled project (Scala 3.7.2, JVM (21))
Hello, World!
```

# Download Spark 

First, the [location](https://dlcdn.apache.org/spark/spark-4.0.0/spark-4.0.0-bin-hadoop3.tgz) has to be installed on the computer via the [bash script](./install_spark.sh).</br>
```bash
bash install_spark.sh
```
and go to the folder.</br>
```bash
cd spark-4.0.0-bin-hadoop3
```
 # The SparkSession

After that, via the following code block activate scala.</br>

```bash
./bin/spark-shell
```
Via the following code block activate pyspark.</br>

```bash
./bin/pyspark
```
You control your Spark Application through a
driver process called the SparkSession. The SparkSession instance is the way Spark executes
user-defined manipulations across the cluster. There is a one-to-one correspondence between a
SparkSession and a Spark Application. In Scala and Python, the variable is available as spark
when you start the console. Let’s go ahead and look at the SparkSession in both Scala and/or
Python.[1]</p>

For scala:
```bash
scala> spark
```

Output:
```bash
val res1: org.apache.spark.sql.SparkSession = org.apache.spark.sql.classic.SparkSession@68886059
```

For python:

```bash
spark
```

Output:
```bash
<pyspark.sql.session.SparkSession object at 0x7f3a969ac4a0>
```
# References

[1] https://raw.githubusercontent.com/rameshvunna/PySpark/master/Spark-The%20Definitive%20Guide.pdf