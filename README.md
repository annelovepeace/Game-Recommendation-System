## Summary
Recommendation system is a subclass of information filtering system that seek to <br>
predict the “rating” or “preference” that a user would give to an item. <br>
The implementation of Recommendation System is very popular in recent years, <br>
specifically, it has been widely used in game platforms. <br>
This recommendation system project is based on the Steam Platform,<br>
aim to analyze users data and games data and design a recommendation system <br>
according to multiple machine learning models.

## Workflow
- Data collection (web crawling)
- Feature selection
- Data engineering
- Data modeling

### Data Collection
1. select 5000 Steam ID
2. develop a web crawler in Python to get Steam users' inventory and <br>
playing behaviors from Steam API using these 5000 IDs
3. get Steam game app IDs and stats from Steamspy API
4. develop a web crawler in Python to get Steam games' details

### Feature Selection
1. scan 300+ features
2. select useful features including price, name, score, platfrom, release date, etc.

### Data Engineering
1. extra data from original txt or json files
2. make necessary transformation on selected features and fill blank values
3. write processed data to MySQL database

### Data modeling
1. Popularity based
2. Content based (tfidf)
3. Collaborative filtering - item based
4. Collaborative filtering - user based (Alternating Least Squares in Pyspark)    
