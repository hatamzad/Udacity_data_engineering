

Project description: 

This project is about dimensional modelling concepts in Postgres and data modeling with extract transform and load datas


Database design: 

Using to analize the data By using SQL and the star scheme also using a relational database, Sparkify can also perform ad analysis of its database.


ETL Process:

Use Sparkify to analyze their data, a Relational Database Schema was created, which can be filled with an ETL pipeline.
The so-called star scheme enables the company to view the user behaviour over several dimensions. The fact table is used to store all user song activities that contain the category "NextSong". Using this table, the company can relate and analyze the dimensions users, songs, artists and time.

Fill the relational database, an ETL pipeline is used, which makes it possible to extract the information from the log files of the user behaviour also the convert data into the schema.

Fact Table & Dimension Tables



Project Repository files: 

data: Folder containing data of songs and logs
create_tables.py: Python script to perform SQL-Statements for (re-)creating database and tables
sql_queries.py: Python script containing SQL-Statements used by create_tables.py and etl.py
etl.py: Python script to extract the needed information from Song and Log data inside the data folder and parsing/inserting them to the created database schema and tables.



How To Run the Project: 

you must run the two files in the order that they are listed here

To create tables:

python3 create_tables.py

To fill tables via ETL:

python3 etl.py
