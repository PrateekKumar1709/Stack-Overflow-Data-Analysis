# Stack-Overflow-Data-Analysis


## Overview:

This project aims to analyze stack overflow data using various big data technologies like PySpark, Elasticsearch, and Kibana. The data used is from Stack Overflow API which contains Stack Overflow content, including posts, votes, tags, and badges. The analysis of this data can help us answer some questions about the programmer’s general preferences.


## Architecture:

<img width="1000" alt="Assignment 1 architecture diagram (2)" src="https://github.com/PrateekKumar1709/Stack-Overflow-Data-Analysis/blob/main/screenshot/architecture.png">

## Implementation:

Following points decribe how the project has been implemented:

1. The raw data is fetched from Stack Overflow API.
2. This data is then loaded into PySpark for pre-processing and cleaning.
3. The processed data is then ingested into Elasticsearch index.
4. The integration between Elasticsearch and PySpark is done via the Elastic ES-Hadoop library which is an open-source, stand-alone, self-contained, small library that allows Hadoop jobs to interact with Elasticsearch. Elasticsearch-hadoop provides native integration between Elasticsearch and Apache Spark, in the form of an RDD (Resilient Distributed Dataset) (or Pair RDD to be precise) that can read data from Elasticsearch.
5. Finally we use Kibana to query data from the Elasticsearch index and create an interactive dashboard to visualise the data and show metrics like popularly discussed topics, post count over time, #questions, #answers, #views, #accepted answers and #comments etc.

## Dashboard:

Below is a sample view of the developed Kibana dashboard.

<img width="1000" alt="Assignment 1 architecture diagram (2)" src="https://github.com/PrateekKumar1709/Stack-Overflow-Data-Analysis/blob/main/screenshot/kibana_dashboard.png">
