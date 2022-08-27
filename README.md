<h1>Project: Data Modeling with Cassandra</h1>


<h3>Introduction</h3>
A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analysis team is particularly interested in understanding what songs users are listening to. Currently, there is no easy way to query the data to generate the results, since the data reside in a directory of CSV files on user activity on the app.

They'd like a data engineer to create an Apache Cassandra database which can create queries on song play data to answer the questions, and wish to bring you on the project. Your role is to create a database for this analysis. You'll be able to test your database by running queries given to you by the analytics team from Sparkify to create the results.


<h3>Project Description</h3>
In this project, you'll apply what you've learned on data modeling with Apache Cassandra and complete an ETL pipeline using Python. To complete the project, you will need to model your data by creating tables in Apache Cassandra to run queries. You are provided with part of the ETL pipeline that transfers data from a set of CSV files within a directory to create a streamlined CSV file to model and insert data into Apache Cassandra tables.

We have provided you with a project template that takes care of all the imports and provides a structure for ETL pipeline you'd need to process this data.


<h3>Data files</h3>
    
<code>The data are stored as a collection of csv files.</code>

Here is example of the data

 https://github.com/ThiagoPositeli/project-udacity-cassandra/blob/main/Captura%20de%20Tela%202022-08-27%20%C3%A0s%2012.35.19.png


<h3>ETL pipeline</h3>

The ETL pipeline and data modeling they are running in a single jupyter notebook: Project_1B_Project_Template.ipynb.

ETL copies data from the datas on csv files to a single csv file event_datafile_new.csv which is used to populate the denormalized Cassandra tables optimised for the 3 queries above. 
The 3 tables in the model are named after the song play query they are created to solve:

<code>songinfo_by_session_by_item includes artist, song title and song length information for a given sessionId and itemInSessionId.</code>

<code>songinfo_by_user_by_session includes artist, song and user for a given userId and sessionId.</code>

<code>userinfo_by_song includes user names for a given song.</code>


