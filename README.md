# Docker-Spark-HDFS-Kafka
Repository containing docker-compose files for quickly setting up a docker cluster consisting of Spark, HDFS, Kafka.

## Requirement
Docker Desktop must be preinstalled.

## How to deploy
Navigate to the folder containing `docker-compose.yml` file, type `docker-compose up -d`.

Services available at:
* Jupyter Lab: [localhost:8888](http://localhost:8888)
* Spark: [localhost:8080](http://localhost:8080)
* Hadoop: [localhost:9870](http://localhost:9870)

## Connect Scrapy Item Pipeline to Kafka Cluster
Please refer to [os-scrapy-kafka-pipeline](https://pypi.org/project/os-scrapy-kafka-pipeline/). .

Default kafka brokers' addresses are ["192.168.1.5:9092","192.168.1.5:9093","192.168.1.5:9094"] (configured in `docker-compose.yml`).

## Credits
1. [big-data-europe/docker-hadoop](https://github.com/big-data-europe/docker-hadoop)
2. [wurstmeister/kafka-docker](https://github.com/wurstmeister/kafka-docker)
3. [cluster-apps-on-docker/spark-standalone-cluster-on-docker](https://github.com/cluster-apps-on-docker/spark-standalone-cluster-on-docker)
4. [elasticsearch](https://www.elastic.co/guide/en/elasticsearch/reference/current/docker.html)

## Other Dockers
`docker-compose.yml` files for deploying elasticsearch & kibana cluster, as well as other individual clusters are also provided. 
