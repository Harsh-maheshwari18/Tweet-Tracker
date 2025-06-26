# Tweet-Tracker
# 🐦 Tweet Tracker: Twitter Sentiment Analysis for Public Policy


Tweet Tracker is a Python-based mini-project that extracts tweets related to specific public policy issues and performs sentiment analysis using NLP tools like TextBlob and VADER. This project helps explore how social media sentiment reflects public opinion on policies such as #Budget2025 or #Agnipath.

---

## 📌 Objectives

- Learn Python for data analysis
- Extract real-time Twitter data using `snscrape`
- Clean and preprocess tweet text for analysis
- Apply sentiment analysis tools to classify tweets
- Analyze public opinion patterns

---

## 🛠️ Tools & Libraries Used

- Python 3
- [snscrape](https://github.com/JustAnotherArchivist/snscrape) — for tweet extraction
- Pandas — for data handling
- Regex (`re`) — for cleaning text
- [TextBlob](https://textblob.readthedocs.io/) — sentiment polarity
- [VADER Sentiment](https://github.com/cjhutto/vaderSentiment) — sentiment analysis
- Google Colab — development environment

---

## 📈 Workflow

### Week 1: Setup & Data Collection
- Learned Python basics (lists, dictionaries, functions, Pandas)
- Used `snscrape` to extract tweets with hashtags like `#Budget2025`

### Week 2: Data Cleaning
- Removed URLs, mentions, hashtags, emojis, and special characters
- Converted text to lowercase
- Tokenized and filtered stopwords (optional)
- Added `clean_text` column to dataset

### Week 3: Sentiment Analysis
- Applied TextBlob and VADER to cleaned tweets
- Generated sentiment scores and labeled each tweet as **Positive**, **Neutral**, or **Negative**
- Analyzed keyword patterns and sentiment distributions

---

## 🧪 Sample Output

| original_text | clean_text | sentiment_score | sentiment_label |
|---------------|------------|------------------|------------------|
| I love the new budget reforms! 🇮🇳 | i love the new budget reforms | 0.5 | Positive |
| Budget 2025 is disappointing... | budget 2025 is disappointing | -0.6 | Negative |

---

## 📂 Project Structure

📁 Tweet-Tracker/
├── tweet_tracker.ipynb # Main notebook
├── week2_cleaned.csv # Cleaned tweet data
├── week3_sentiment_output.csv # Final dataset with sentiment
└── README.md # Project documentation

yaml
Copy
Edit

---

## 🚀 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/tweet-tracker.git
   cd tweet-tracker
Open the notebook in Google Colab or run locally.

Install dependencies:

bash
Copy
Edit
pip install snscrape textblob vaderSentiment pandas
Run all cells in tweet_tracker.ipynb

📊 Future Improvements
Add interactive visualizations (e.g., sentiment timeline, word clouds)

Support for multiple hashtags/topics

Integrate with Twitter API for real-time data (if needed)

Extend to classify sarcasm or misinformation

