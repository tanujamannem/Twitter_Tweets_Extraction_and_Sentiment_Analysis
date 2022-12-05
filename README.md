# Twitter_Tweets_Extraction_and_Sentiment_Analysis

**Task:** The following are the tasks to perform.

**Objective 1:** Get the most frequent entities from the tweets.

**Objective 2:** Find out the sentiment/polarity of each author towards each of the entities.

**Technology used:** Natural Language Processing, Data Pre-processing, Sentiment Analysis, Entities Extraction, TextBlob library.

**Approach for the Solution:** Data Preprocessing is very important for this data because this is text data.

**Procedure:** 
1. Loading the Json File

2. Conversion of Rawdata into Pandas DataFrame.

3. Defining Function for furthur process.

4. Cleaning the Data.

5. Extracting the entities from the tweets and finding their frequency.

6. Converted to CSV file (objective1.csv)(Solution of objective 1).

7. Finding Sentiment of the tweets based on tweet entities and author.

8. Extracted wanted columns based on the output and converted to csv file (objective2.csv)(Solution of objective 2).

**Explantion of total Process:**

**1. Loading the Json File:** Loaded the json file. Observed the data. Data cleaning is the main step in this process.The raw data helped to understand the problem statement and insights in the data.

**2. Conversion of Rawdata into Pandas DataFrame:** To Start the solution for the problem, we have to convert the data in to understandable way. I converted the rawdata into Pandas dataframe.

**3. Defining Functions:** Defined the function for furthur implementation of the process.

**4. Data Preprocessing:** Cleaning of data plays major role in this problem. I cleaned tweets data like removing unwanted elements from the data, Those are hashtags, url links, numbers in the tweets, removing stop words and words less than two characters and etc.

**5. Extracting Entities and Frequency:** Extracting entities also major task in this. There are so many ways to extract entites like Tokenization, stemming, Lemmatization. But, for these processess it will extract only words. This process wont give effective meaning of tweets. For this, I used TextBlob library's Noun_Phrase extractor. By using this, the entities are in some length of words and it given idea about tweets also.

**6. Solution of Objective1:** For this, I created new dataframe and extracted tweets entities and frequency of entities based on output and converted to csv file.

**7. Sentiment Analysis based on Entitites:** I created copy of task1 in another dataframe and used in this. Used NLTK package Sentiment analyzer to extract the sentiments i.e. Positive, Negative, Neutral. Created new column with polarity and added these categories.

**8. Solution of Objective2:** Extracted wanted columns from the dataset based on the sample output, those are tweet author, entities and polarity. converted the dataframe into csv file.

**Difficulties & Short comings I approached:**

1. The main step with this data is Data Cleaning. I spent good time to clean the data.

2. I faced the difficulty to extract the entities. The short coming is extracting the noun phrases from tweets. With the help of TextBlob library Extracted entities from the tweets.

3. Used NLTK package Sentiment analyzer for extracting the sentiments of entities.

4. The short coming is, related to different language text data. For time being, I ignored translation of another language text in to English.
