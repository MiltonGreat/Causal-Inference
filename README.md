# Sentiment Analysis & Stock Market Prediction

![screenshot-localhost_8888-2025 03 31-16_48_41](https://github.com/user-attachments/assets/d29021ac-7673-49c0-94e8-b0aab0550320)

### Project Overview

This project investigates whether news sentiment influences stock market movements using Granger causality tests. We analyze financial news headlines using VADER and TextBlob sentiment analysis and compare sentiment trends with S&P 500 daily returns.

### Methodology

1. Extract News Sentiment
- Collect financial news headlines
- Apply VADER & TextBlob to extract sentiment scores
- Aggregate daily sentiment averages

2. Get S&P 500 Data
- Retrieve daily close prices
- Calculate percentage returns

3. Merge and Process Data
- Align sentiment scores and stock returns
- Remove missing values
- Check for stationarity (ADF Test)

4. Causality Testing (Granger Tests)
- Does sentiment influence stock returns?
- Does stock movement affect sentiment?

5. Visualization & Interpretation
- Time series plots of sentiment vs. stock returns
- Autocorrelation & cross-correlation
- Scatter plots for insights

### Key Findings

- Both sentiment and stock returns are stationary (p-value < 0.05).
- No significant causality found between sentiment and stock returns (p-values > 0.05).
- Stock returns may be driven by broader economic factors rather than sentiment alone.

### Future Enhancements

1. Include Social Media Data (Twitter, Reddit, earnings calls).
2. Use Deep Learning Models (BERT, LSTMs for better sentiment extraction).
3. Check Nonlinear Relationships (Machine learning models like Random Forest).
4. Analyze Specific Sectors (Tech, Crypto may react differently to sentiment).

### Source

![Financial News Headlines Data from Kaggle](https://www.kaggle.com/datasets/notlucasp/financial-news-headlines#%20Sentiment%20Analysis%20in%20Finance)
