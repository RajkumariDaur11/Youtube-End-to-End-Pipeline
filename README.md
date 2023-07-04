# Youtube | End to End Pipeline

## Overview
In this project, I have designed and implemented an end-to-end data pipeline that consists of several stages:
1. Extracted Youtube data in the JSON and CSV format and loaded it into S3.
2. Crawled the data from S3 to Athena using AWS Glue.
3. Transfomed the raw data into Parquet format using AWS Lambda.
4. Performed pre processing on the formatted parquet data on Athena.
5. Build ETL jobs in AWS Glue using Spark to merge formatted data from different raw formats into a cleansed bucket. 
6. Set up a trigger in AWS Lambda to automate the formatting request.
7. Built ETL pipeline to pull the data in reporting database on Athena for reporting.


## Dataset-  
This Kaggle dataset contains statistics (CSV files) on daily popular YouTube videos over the course of many months. There are up to 200 trending videos published every day for many locations. The data for each region is in its own file. The video title, channel title, publication time, tags, views, likes and dislikes, description, and comment count are among the items included in the data. A category_id field, which differs by area, is also included in the JSON file linked to the region.

Raw Data - https://www.kaggle.com/datasets/datasnaek/youtube-new

## Technology Used 
* Language: Spark, Python, SQL
* Extraction and transformation: Athena, AWS Lambda

* Storage - Amazon S3
* Integration Service - AWS Glue

 ## Data Pipeline Architecture
https://github.com/RajkumariDaur11/Youtube-End-to-End-Pipeline/blob/main/Data%20Architecture.jpg




