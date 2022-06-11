# Project 2- ETL Magic The Gathering
Georgia Tech Data Analytics Bootcamp Project 2: Extract, Transform, and Load
## Collaborators
Dan Davies (https://github.com/Dans1451)  and Prakhyath Bagavatula (https://github.com/Prakb2401)

### Proposal
This project’s objective was to create a database of all Magic The Gathering cards and their attributes. With this information someone who wants to buy sets of cards as a whole can find the pricing of specific cards through TCGplayer, an online market to buy and sell cards. We extracted all the cards from Scryfall and MTGjson. We found that both data sources had some redundant information but also had information unique to each source. We will use Pandas to transform the data as well as clean and merge the data into one database. We will load our database into MongoDB and create a document database and compile tables from our data sources. For installation of this project you need Pandas, to clean data, Pymongo and Mongodb, to load the data, and a working Python 3 environment. 

### Sources
Data source 1- https://scryfall.com/docs/api - json file,
Data source 2- https://mtgjson.com/ - csv files

### Usage
The Scryfall JSON file is in a compressed folder because it was to big to upload normally. So when beginning this project you must extract the JSON from its compressed folder. Following there we set up the MongoDB client and started to clean the data. You can use Pandas to delete any redundant information between the cards.csv and the Scryfall.json sources. When you are ready to load the database into MongoDB the database must be called Mtg_Cards and collections must be named 
MTG_Cards.

### Extract
* We started by extracting a json file from Scryfall api website 6/6/2022.
* For our second data source we found MTGjson through kaggle and scrape card information to obtain a csv file 6/6/2022.
* Some issues we had in this stage included the json file being to big to upload into GitHub so we compressed the file then uploaded it. When extracting the json file you must extract the file from the compressed folder.

### Transform
* We used Pandas to clean remove unnecessary columns, combine teh datasets and clean null values
* We used Pandas to remove any redundant information between the data sources

### Load
* We took a sample of 100 cards from the dataframe before uploading it MongoDB.
* Load the final dataframe into MongoDB useing PyMongo
* Some issues we faced during this stage was that the dataframe was to large to upload into MongoDB. Dan took sample of the dataframe and then created a loop to add a card one by one into the database.

### Results
The outcome of the project created a database containing a sample of our larger dataframe. We have information of over 67,000 cards but in the database only 100. This is because of hardware limitations. However our purpose for this project is for anyone to be able to find completed card sets efficently and our dataframe accomplishes this. With the information in our dataframe anyone can input completed card sets into [TCGplayer](https://www.tcgplayer.com/massentry?_gl=1%2aolor6j%2a_gcl_aw%2aR0NMLjE2NTQ1NTU0NDguQ2p3S0NBand5X2FVQmhBQ0Vpd0EySUhIUUhub0RqeTBVbld0WW8zX1hkQ1N6ZXIwYmZWeThLLWp5Z3gwU2J1ejc4SFE3VjNoYU1waDNCb0N6RUFRQXZEX0J3RQ)

### License
MIT License

Copyright (c) [2022] [Dan Davies, Prakhyath Bagavatula]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.



