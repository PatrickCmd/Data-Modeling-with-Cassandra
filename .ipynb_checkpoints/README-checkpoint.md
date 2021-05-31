# Data Modeling with Cassandra

This is a data modeling project created under Data Modeling With Apache Cassandra for [Data Engineer Nanodegree](https://www.udacity.com/course/data-engineer-nanodegree--nd027)

## Project Overview.

A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app.

The project is about data modeling with Apache Cassandra and complete an ETL pipeline using Python. There is modeling data by creating. tables in Apache Cassandra to run queries. The ETL pipeline transfers data from a set of CSV files within a directory to create a streamlined CSV file used to model and insert data into Apache Cassandra tables as in the project notebook.

## Datasets

For this project will be working on dataset: **event_data**. The directory of CSV files partitioned by date. Here are examples of filepaths to two files in the dataset:

```
event_data/2018-11-08-events.csv
event_data/2018-11-09-events.csv
```

## Project Steps

### Processing steps
- Process files in the **event_data** directory to created a new streamlined data file **event_datafile_new.csv**
- Process the **event_datafile_new.csv** dataset to a create a denormalized dataset.
- Model the data tables keeping in mind the queries you need to run.
- Load the data into tables created in Apache Cassandra and run queries.

### Modeling your NoSQL database or Apache Cassandra database
- Design tables to answer the queries outlined in the project template
- Write Apache Cassandra **CREATE KEYSPACE** and **SET KEYSPACE** statements
- Develop **CREATE** statement for each of the tables to address each question
- Load the data with **INSERT** statement for each of the tables
- Include **IF NOT EXISTS** clauses in the **CREATE** statements to create tables only if the tables do not already exist. Recommended also to include **DROP TABLE** statement for each table, this way you can run drop and create tables whenever you want to reset your database and test your ETL pipeline
- Test by running the proper select statements with the correct** WHERE** clause

## Contents
- **event_data**: The directory of CSV files partitioned by date
- **project_notebook**: The notebook has steps for the ETL pipeline from data processing, data modeling in Cassandra database and loading the data into the database tables.