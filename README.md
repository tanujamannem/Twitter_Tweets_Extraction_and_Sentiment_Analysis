# 🌐 Twitter Tweet Extraction & Sentiment Analysis
A complete NLP workflow to extract, clean, analyze, and classify tweets from a JSON dataset.

---

## 📌 Project Overview  
This project processes raw tweets and converts them into structured insights using Natural Language Processing.  
It extracts key entities from tweets, identifies sentiment, and prepares clean datasets for reporting or machine-learning tasks.

---

## 🔍 What This Project Does  
- Loads tweets from a JSON file and converts them into a structured DataFrame.  
- Cleans tweet text by removing URLs, mentions, hashtags, punctuation, and stopwords.  
- Normalizes the text (lowercasing, spacing) for NLP processing.  
- Extracts important noun phrases using TextBlob to identify key topics.  
- Counts the frequency of extracted entities and saves the output.  
- Performs sentiment analysis using VADER (positive, negative, neutral scores).  
- Classifies each tweet as **Positive**, **Negative**, or **Neutral**.  
- Exports clean datasets for further analysis.

---

## 🛠️ Technologies Used  
- Python  
- NLTK  
- TextBlob  
- VADER Sentiment Analysis  
- Pandas / NumPy  

---

## 🧠 Workflow Summary  
1. **Tweet Extraction**  
   - Reads the `tweets.json` file and flattens nested structures.

2. **Text Cleaning**  
   - Removes URLs, mentions, hashtags, numbers, symbols, stopwords.  
   - Converts text to lowercase and removes extra whitespace.

3. **Entity Extraction**  
   - Uses TextBlob to extract noun phrases.  
   - Generates a frequency count and stores results in `objective1.csv`.

4. **Sentiment Analysis**  
   - Uses VADER to generate sentiment scores.  
   - Labels tweets as Positive, Negative, or Neutral.

5. **Final Output**  
   - Adds cleaned text, entities, and sentiment labels.  
   - Saves final processed data in `objective2.csv`.

---

## 📁 Output Files  
- **objective1.csv** → Noun phrase counts  
- **objective2.csv** → Cleaned tweets with sentiment scores  

---

## 📊 Example Output Columns  
- tweet_text  
- clean_text  
- noun_phrases  
- sentiment_positive  
- sentiment_negative  
- sentiment_neutral  
- compound_score  
- sentiment_label  

---

## 🎯 Project Purpose  
- Helps understand public sentiment on any topic.  
- Shows a full real-world NLP pipeline.  
- Useful for dashboards, topic analysis, or ML model preparation.
