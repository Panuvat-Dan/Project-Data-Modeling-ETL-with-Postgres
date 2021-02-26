# Project-Data-Modeling-ETL-with-Postgres

## Objective of this project

In this project mainly focused on how to create and drop table by similating work on start up companee name Sparktify and the company need to analyze
the data.Thus, as a data engineer requires skill to collect and transform and load into postgres database. The pipeline is not automated schduling by airflow yet. 

## Project description

In this project, you'll apply what you've learned on data modeling with Postgres and build an ETL pipeline using Python. To complete the project, you will need to define fact and dimension tables for a star schema for a particular analytic focus, and write an ETL pipeline that transfers data from files in two local directories into these tables in Postgres using Python and SQL.

## Database schema 

This project aims to utilize star schema by having fact table as songplays and the rest are dimention tables as picture below,
![alt text](https://github.com/Panuvat-Dan/Project-Data-Modeling-ETL-with-Postgres/blob/main/Entity_diagram.png)

## Files

\1.data (log,song data)
\2.create_tables.py
\3.sql_queries.pynb
\4.elt.pynb
\5.etl.py
\6.test.pynb

## ETL pipeline 

Before scripping ETL.py it has been tested on ETL.pynb to test the loading 

After testing,ETL.py will work as following for processing the data:

-Connect to the sparkify database and it will drop and create all the tables.
-Parse out each json file from log&song data then load all of the files into dataframe.
-All songs from Song_data and Log_data will be loaded into the tables on .

### Dataset

* Song data example
  > song_data/A/B/C/TRABCEI128F424C983.json
  > song_data/A/A/B/TRAABJL12903CDCF1A.json
* Log data example
  >log_data/2018/11/2018-11-12-events.json
  >log_data/2018/11/2018-11-13-events.json
* interface
  >{
    "num_songs": 1,
    "artist_id": "ARJIE2Y1187B994AB7",
    "artist_latitude": null,
    "artist_longitude": null,
    "artist_location": "",
    "artist_name": "Line Renaud",
    "song_id": "SOUPIRU12A6D4FA1E1",
    "title": "Der Kleine Dompfaff",
    "duration": 152.92036,
    "year": 0
    }
## How to run

* 1.Run create_tables.py from terminal to set up the database and tables.
* 2.Run etl.py from terminal to process and load data into the database.
* 3.Launch test.ipynb to run validation and example queries.

## Credit 

I need to thank Udacity for the dataset given as Log_data and song_data and the guideline throughout this project.
Moreover,Lucidchart website provide a good source to create Entity diagram.
