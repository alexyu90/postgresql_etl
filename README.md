## Project Overview

This project is an excercise for data modeling with Postgres and building an ETL pipeline using Python. Fact and dimension tables for a star schema is defined, and an ETL pipeline is written to transfer data from files in two local directories into tables in Postgres using Python and SQL.

The dataset is a simulated dataset of a spotify-like startup. It includes songplay logs, song details and artist details. The data is modeled using a star scheme, with 1 fact table "songplays" and 4 dimension tables "users", "songs", "artists" and "time".


## Libraries Used:
The following libraries are used in this project:
- PostgreSQL: psycopg2
- PyData: pandas
- Utilities: glob, os


## How to Run:
- run create_tables.py to initialize (or drop previous) database and create empty tables
- run etl.py to utilize etl pipeline to extra data from files to database
- use test.ipynb to query database 


## Files Description:
- create_tables.py: drops existing database and tables, and creates new database and tables;
- etl.ipynb: a walkthrough template with detailed instructions for creating the etl.py file;
- etl.py: a etl pipeline that extracts data from files to database and create 5 tables: songplays, users, songs, artists and time;
- sql_queries.py: containing SQL commands to drop and create tables, insert records and query database;
- test.ipynb: a jupiter notebook with magic commands to query database.


## Acknowledgement 

Credits to Udacity for the templates.