# Sparkify

## Project Scope

This project is for a startup called Sparkify who wants to analyze the data they've been collecting (songs and user activity) on their new music streaming app. 

The main focus is on what songs the users are listening to.

Within this project, I have created a Postgres Database locally and I will insert data from JSON metadata generated by the music streaming app.


### Example Song Data

```
{
  "artist_id": "ARD7TVE1187B99BFB1",
  "artist_latitude": NaN,
  "artist_longitude": NaN,
  "artist_location": "California - LA",
  "artist_name": Casual,
  "duration": 218.93179,
  "num_songs": 1,
  "song_id": "SOMZWCG12A8C13C480",
  "title": "I Didn't Mean To",
  "year": 2010
  
}
```


### Example Log Data

```
{
  "artist": "Des'ree",
  "auth": "Logged In",
  "firstName": "Kaylee",
  "gender": "F",
  "itemInSession": 1,
  "lastName": "Summers",
  "length": 246.30812,
  "level": "free",
  "location": "Phoenix-Mesa-Scottsdale, AZ",
  "method": "PUT",
  "page": "NextSong",  
  "registration": 1540344794796,
  "sessionId": 139,
  "song": "You Gotta Be",
  "status": 200  
  "ts": 1541106106796,
  "userAgent": "Mozilla/5.0 (Windows NT 6.1; WOW64)",
  "userId": 8,
}
```

## ETL

Python will be used to create the ETL pipeline which is first tested in the jupyter notebook here: [GitHub](https://github.com/Ryan-Ashton/Udacity-Data-Engineering/blob/main/etl.ipynb)

The main files utilised are:
- create_tables.py (to create the tables)
- sql_queries.py (to organise the SQL queries)
- etl.py (to process the data) 


## Schema

The visual representation of the Database Schema: 

![picture](img/Star_Schema.JPG)
