# Project-Data-Modeling-ETL-with-Postgres

## Objective of this project

In this project mainly focused on how to create and drop table by similating work on start up companee name Sparktify and the company need to analyze
the data.Thus, as a data engineer requires skill to collect and transform and load into postgres database. The pipeline is not automated schduling by airflow yet. 

## Project description

## Database schema 

This project aims to utilize star schema by having fact table as songplays and the rest are dimention tables as picture below,
![alt text](u)

## Files

1.data (log,song data)
2.create_tables.py
3.sql_queries.pynb
4.elt.pynb
5.etl.py
6.test.pynb

## ETL pipeline 

Before scripping ETL.py it has been tested on ETL.pynb to test the loading 

After testing,ETL.py will work as following for processing the data:

-Connect to the sparkify database and it will drop and create all the tables.
-Parse out each json file from log&song data then load all of the files into dataframe.
-All songs from Song_data and Log_data will be loaded into the tables on .

## Credit 

I need to thank Udacity for the dataset given as Log_data and song_data and the guideline throughout this project.
Moreover,Lucidchart website provide a good source to create Entity diagram.
