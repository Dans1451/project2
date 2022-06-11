# Project 2- ETL Magic The Gathering
Georgia Tech Data Analytics Bootcamp Project 2: Extract, Transform, and Load
## collaborators
Dan Davies (https://github.com/Dans1451)  and Prakhyath Bagavatula (https://github.com/Prakb2401)

### Proposal
This project’s objective was to create a database of all Magic The Gathering cards and their attributes. With this information someone who wants to buy sets of cards as a whole can find the pricing of specific cards through TCGplayer, an online market to buy and sell cards. We extracted all the cards from Scryfall and MTGjson. We found that both data sources had some redundant information but also had information unique to each source. We will use pandas to transform the data as well as clean and merge the data into one database. We will load our database into MongoDB and create a relational database and compile tables from our data sources. For installation of this project you need Pandas, to clean data, Pymongo and Mongodb, to load the data, and a working Python 3 environment. 

### Sources

Data source 1- https://scryfall.com/docs/api - json file,
Data source 2- https://mtgjson.com/ - csv files

### Extract
* We started by extracting a json file from Scryfall api website. 
* For our second data source we found MTGjson through kaggle and scrape card information to obtain a csv file.
* Some issues we had in this stage included the json file being to big to upload into GitHub so we were able to compress the file then upload it.

### Transform
* We used Pandas to clean the data and make it more manageable. 
* We used Pandas to remove any redundant information between the data sources
* We used Pandas to merge the data into one table

### Load
* Load the final dataframe into MongoDB 
deleted this later
