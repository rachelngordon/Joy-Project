# Joy-Project
Research project analyzing the use of joy on Twitter throughout the pandemic using NLP

## Data Collection

### TwitterScraping.py
Data was scraped from Twitter using the snscrape package
Tweets located near Chicago from September 2019 through January 2022 were collected
Data was originally stored as separate json files for each day


## Preprocessing

### CombineJSONFiles.py
The separate json files for each day were combined into a larger file for a given month

### ReformatJSON.py
The separate json files for each month were reformated to add a "tweets" object including all of the tweets in the file
This was done so that the files could easily be read using the json.load() function

### AddJoyFlag.py
Add "ijoy" column to the data indicating whether or not a tweet contains the word "joy"
Create separate month files with only tweets containing the word "joy"

### TextCleaning.ipynb
Clean the tweets by removing urls, hashtags, punctuation, stopwords, and converting to all lowercase
Add a column to the data for the clean tweets that have been stemmed
Add a column for the meanings of the emojis that are included in each tweet

### CombineCleanFiles.ipynb
Combine all of the cleaned data into one larger filer called "allData"



