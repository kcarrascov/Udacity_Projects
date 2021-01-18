# Project1: Data modeling with Postgres
 
 
The project is contextualized in a startup called Sparkify that wants to analyze the data they have been collecting about songs and user activity in their new music streaming application and are interested in understanding what songs are being played. The data resides in a directory of JSON records about user activity in the application as well as a directory with JSON metadata on the songs in your application so there is currently no easy way to accomplish this.

Thus, the mission will be to create a Postgres database with tables designed to optimize queries on song playback analysis and that will lead you to the project, making use of the tools and knowledge learned in the course on data modeling with Postgres and create an ETL pipeline using Python.

For the project, the instructions will be followed and the files delivered will be taken for their completion and subsequent verification of the correct functioning of the objective. 

The set of data delivered with which they will work are the following tables:

**1.Songplays:** Here you can find information about the records in the log data associated with the playback of songs (NextSong)
(songplay_id, start_time, user_id, level, song_id, artist_id, session_id, location, user_agent)

**2.Users:** User information in the application
(user_id, first_name, last_name, gender, level)

**3.Songs:** Information about the available songs
(song_id, title, artist_id, year, duration)

**4.Artists:** Information of the artists found in the music database
(artist_id, name, location, latitude, longitude)

**5.Time:** Time stamps of the records in the songs 
(start_time, hour, day, week, month, year, weekday)

Then, with this information we should proceed to the project if, finding the necessary files in the workspace. The steps and files considered are the following:

**1.Create Tables**

 1.1 sql_queries.py file : 
 Using the INSERT AND DROP commands.
 This file, using Python, contains all the declarations to create the fact and dimension tables and data used during the loading process. The declarations implemented here        (CREATE TABLE and INSERT) are imported and used in the files that follow and the following ones.

 1.2 créate_tables.py file: 
 This file will create the Postgres database and each of the necessary tables, connecting them, eliminating the existing ones and creating the fact and dimension   tables.Then, in the following main file the data will be completed

 1.3 test.ipnyb file: 
 Confirmation of correct table and data creation
 This file will be a verification test to check the correct execution of the table creation and the data inserted


**2.Creation of ETL processes:**

 2.1 etl.ipnyb file: 
 In this file you must follow the instructions for the creation of the ETL process for each table 

 2.2 test.ipynb file: confirmation that the data was correctly inserted 
 This file will be a verification test to check the correct execution of the table creation and the data inserted

 2.3 create.table.py: used to restore tables before the corresponding executions



**3.Create ETL pipeline:**

 3.1 etly.py file: 
 Use the completion in the etl jupyter of the data processing
 Here the ETL process will start and the table with the data will be completed. The ETL process is implemented by extracting the raw data found in the JSON file, transforming it and loading it into the previously created tables

 3.2 test.ipynb file: 
 Confirm correct records in tables


**4.Documentation process:**

 4.1 README.md file: This file analyzes the purpose and defines what has been done for the design of your database schema and ET pipeline
