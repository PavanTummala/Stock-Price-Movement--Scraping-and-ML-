# Stock-Price-Movement--Scraping-and-ML-

## Overview
This project analyzes Reddit sentiment to predict AAPL stock price movements. By leveraging natural language processing and machine learning techniques, we achieved 79.5% accuracy in predicting daily stock price directions.

## Project Structure
```
├── data/                       # Contains input and processed data
├── notebooks/                  # Jupyter notebooks for analysis and experimentation
│   ├── 01_scraping.ipynb      # Reddit scraping script
│   ├── 02_model_training.ipynb # Sentiment analysis and feature engineering
├── requirements.txt           # Python dependencies
├── README.md                  # Project documentation
└── config.py                  # Reddit API credentials
```

## Features
- Reddit data scraping using PRAW API
- Sentiment analysis using FinBERT and VADER
- TFIDF vectorization for text feature extraction
- Multiple ML models (Random Forest, XGBoost, Logistic Regression)
- Rolling sentiment averages and feature engineering

## Installation

1. Clone the repository
```bash
git clone https://github.com/yourusername/Stock-Price-Movement--Scraping-and-ML-.git
cd Stock-Price-Movement--Scraping-and-ML-
```

2. Install dependencies
```bash
pip install -r requirements.txt
```

3. Configure Reddit API credentials
- Create a `config.py` file in the root directory
- Add your Reddit API credentials:
```python
reddit_config = {
    'client_id': 'your_client_id',
    'client_secret': 'your_client_secret',
    'user_agent': 'your_user_agent'
}
```

## Usage

1. Data Collection
- Run `notebooks/01_scraping.ipynb` to collect Reddit posts
- Posts are saved to `data/` directory

2. Model Training
- Run `notebooks/02_model_training.ipynb` for:
  - Sentiment analysis
  - Feature engineering
  - Model training and evaluation

## Results
- Random Forest Classifier: 79.5% accuracy
- XGBoost: 78.9% accuracy
- Logistic Regression: 65.8% accuracy

## Dependencies
- Python 3.8+
- PRAW
- pandas
- scikit-learn
- transformers (FinBERT)
- vaderSentiment
- XGBoost
- yfinance

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License
[MIT](https://choosealicense.com/licenses/mit/)

## Contact
Your Name - youremail@example.com
Project Link: [https://github.com/yourusername/Stock-Price-Movement--Scraping-and-ML-](https://github.com/yourusername/Stock-Price-Movement--Scraping-and-ML-)

