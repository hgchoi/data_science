# Understanding User Behavior

As a data scientist at a game development company, our latest mobile game has two events that I'm interested in tracking: buy a
sword & join guild.

Each has metadata characterstic of such events (i.e., sword type, guild name, etc).

### Tasks

* Instrument my API server to log events to Kafka

* Assemble a data pipeline to catch these events: use Spark streaming to filter select event types from Kafka, land them into HDFS/parquet to make them available for analysis using Presto

* Use Apache Bench to generate test data for my pipeline

* Produce an analytics report where I provide a description of my pipeline and some basic analysis of the events

* Use a notebook to present my queries and findings.

It is understood that events in this pipeline are generated events which make them hard to connect to actual business decisions. 
However, I would like to demonstrate an ability to plumb this pipeline end-to-end, which includes initially generating test data as well as submitting a notebook-based report of at least simple event analytics.
