# Pyspark-ML
Gathers data science and machine learning problem solving using PySpark and Hadoop.

<img src="https://cdn-images-1.medium.com/max/1600/0*8D301fHKliN6r5Km.png" align="right" width="20%">

## Covered

0. Test Pyspark
1. Text classification IMDB dataset using logistic regression
2. Text classification IMDB dataset using multinomial
3. Topic Modelling TFIDF + LDA
4. Word Vector
5. Read Iris csv from Hadoop DFS
6. PCA on Iris dataset
7. MNIST feed-forward sparkflow
8. MNIST CNN sparkflow

## How-to Notebook

1. Run docker compose,
```bash
compose/build
```

2. Copy link from terminal to browser,
```text
pyspark_1  |     Copy/paste this URL into your browser when you connect for the first time,
pyspark_1  |     to login with a token:
pyspark_1  |         http://(537864b567dc or 127.0.0.1):8080/?token=11f413ac6d1d78aa926042779768759ac227a8ebc0e57ecf
```

## How-to Hadoop

Check Hadoop health, [localhost:9870](http://localhost:9870)

<img src="screenshot/localhost-9870.png" width="60%">

Hadoop DFS Web UI, [localhost:9870/explorer.html#/](http://localhost:9870/explorer.html#/)

<img src="screenshot/hadoop-storage.png" width="60%">

Hadoop Node Manager, [localhost:8042/node](http://localhost:8042/node)

<img src="screenshot/localhost-8042.png" width="60%">

## How-to Spark-cluster

1. Run docker compose,
```bash
docker-compose -f docker-compose-cluster.yml up --build --remove-orphans
```

If success,
```text
slave_2   | 2018-11-18 07:57:59 INFO  Worker:54 - Successfully registered with master spark://192.168.128.2:7077
slave_1   | 2018-11-18 07:58:10 INFO  Worker:54 - Successfully registered with master spark://192.168.128.2:7077
```

<img src="screenshot/pyspark-cluster.png" width="60%">
