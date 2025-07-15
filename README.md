# TradeWave
Stock Market Sentiment Analysis


# 📈 Smart Stock Sentiment Analyzer

An AI-powered web application for managing your stock portfolio, receiving sentiment-based alerts, and chatting with an AI assistant for real-time stock insights.

---

## 🌟 Features

- 🔐 User authentication (Login & Sign Up)
- 📁 Manage your personalized stock portfolio
- 💬 Ask AI chatbot about stock prices or sentiments
- 📊 Sentiment alerts based on news & tweets
- 📰 Google News & 🐦 Twitter sentiment analysis
- 🌥 Word cloud generation of news headlines
- 🎨 Smooth UI using Streamlit and Lottie animations

---

## 🛠 Tech Stack

- **Frontend/UI**: Streamlit
- **Backend**: Python
- **Database**: SQLite
- **APIs**: `yfinance`, `feedparser`, Twitter API v2
- **NLP**: VADER Sentiment Analysis
- **Visualization**: Matplotlib, WordCloud

---

## 📂 File Structure

📦 SmartStockSentiment/
├── app.py # Main Streamlit app
├── chatbot.py # Chatbot and stock query handler
├── database.py # SQLite database functions
├── portfoliomanager.py # In-memory portfolio & alerts
├── reccomendar.py # Recommendation logic based on score
├── sentiment_news.py # News scraping & sentiment
├── twitter_sentiment.py # Twitter-based sentiment
├── requirements.txt # Required packages
└── README.md # This file



---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/smart-stock-analyzer.git
cd smart-stock-analyzer
2. Install Required Packages
bash
Copy
Edit
pip install -r requirements.txt
Or install manually:

bash
Copy
Edit
pip install streamlit yfinance feedparser vaderSentiment wordcloud requests streamlit-lottie matplotlib
3. Run the App
bash
Copy
Edit
streamlit run app.py
🔐 Login Info
On your first use, create a username & password to register.

Your portfolio is saved in users.db locally.


 How to Use the Chatbot
You can ask:

What is the price of AAPL?

Give sentiment for TSLA

Tell me recent news about MSFT

The chatbot understands intent (price, news, sentiment) and ticker from your message.

📈 Sentiment Analysis
Uses VADER to score news & tweets.

If sentiment score < -0.1, you get a ⚠️ negative sentiment alert.

Recommendation labels:

🔼 Strong Buy

⬆️ Buy

⏸️ Hold

⬇️ Sell

🔻 Strong Sell

![WhatsApp Image 2025-07-15 at 13 10 58_b127c81a](https://github.com/user-attachments/assets/bcbe3afc-480d-4759-b5ef-249cc75b6b61)

✅ TODO (Enhancements)
 Add historical stock price charts

 Improve intent extraction using NLP

 Cloud deployment via Streamlit Cloud or AWS

 Enable email alerts on sentiment dips
