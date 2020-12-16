# Tracking User Activity

In this project, I've created a service at an ed tech firm that delivers assessments, and now lots of different customers (e.g., Pearson) want to publish their assessments on it. I need to prepare for data scientists who work for these customers to run queries on the data.

### Tasks

Prepare the infrastructure to land the data in the form and structure it needs to be to be queried. I need to:

* Publish and consume messages with Kafka
* Use Spark to transform the messages.
* Use Spark to transform the messages so that I can land them in HDFS
* I have included my docker-compose.yml used for spinning the pipeline.

I've also included the history of my console by running:

```
history > <user-name>-history.txt
```

I ran Spark by running a Jupyter Notebook against a pyspark kernel.

In order to show the data scientists at these other companies the kinds of data that they will have access to, I decided on a few basic business questions that I believed they might need to answer about these data.

### Data

Note on the data: This dataset is a nested JSON file, where I need to unwrap it carefully to understand what's really being displayed. There are many fields that were not important for my analysis, so many were left untouched. The main problem was the multiple questions field. Documentation for reading schema implementation in Spark Here is the documenation from Apache.

### Business Questions Answered

1. How many assesstments are in the dataset?
2. How many people took Learning Git?
3. How many people got As on their exams?
