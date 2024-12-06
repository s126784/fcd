# Football Player Data Analysis Over Time

## Overview
This project builds a data analysis engine that collects, enriches, and analyzes football player data from Transfermarkt and the Portuguese web archive (arquivo.pt). The analysis focuses on understanding player market values, their web presence, and sentiment analysis of historical articles.

## Features
- Web scraping from Transfermarkt for player market values and statistics
- Historical web data collection from arquivo.pt
- Text and sentiment analysis of player-related articles
- Correlation analysis between market values and web presence
- Data visualization and statistical analysis

## Project Structure
```
├── data/                   # Processed data files
│   ├── portugal_*.csv      # Basic player data
│   ├── portugal_*_plus.csv # Enriched player data
│   └── url_content.csv     # Cached web content
├── snapshots/              # Raw data snapshots
│   ├── portugal_*.html     # Transfermarkt HTML snapshots
│   └── *_*.json            # arquivo.pt API responses
└── 126784-project1.ipynb   # Initial data collection and analysis
└── 126784-project2.ipynb   # Text analysis and sentiment analysis
```

## Prerequisites
- Python 3.8+
- Required Python packages:
  ```
  pandas
  numpy
  requests
  beautifulsoup4
  seaborn
  matplotlib
  nltk
  scikit-learn
  trafilatura
  transformers
  torch
  ```

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/s126784/fcd.git
   cd fcd
   ```

2. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Download NLTK data:
   ```python
   import nltk
   nltk.download('punkt')
   nltk.download('stopwords')
   nltk.download('wordnet')
   ```

## Usage

### Part 1: Data Collection and Initial Analysis
1. Set up the web scraping environment
2. Collect data from Transfermarkt using jupyter notebook
3. Query historical web snapshots from arquivo.pt
4. Perform initial data analysis

### Part 2: Text Analysis and Sentiment Analysis
1. Process collected web content
2. Apply sentiment analysis using jupyter notebook
3. Generate enriched features and metrics

## Data Sources
- [Transfermarkt](https://www.transfermarkt.com/): Player market values and statistics
- [arquivo.pt](https://arquivo.pt/): Historical web content archive

## Analysis Results
- Strong correlation between player market values and web presence
- Sentiment analysis reveals relationship between media coverage and market value changes
- Temporal analysis shows evolution of player valuations

## Future Improvements
- Player clustering based on text features
- Advanced time series modeling
- Machine learning for value prediction
- Additional data source integration
- Social media metrics analysis

## References
- Sozen, Y. (2023). Predicting Football Players Market Value Using Machine Learning
- Transfermarkt Documentation
- Arquivo.pt API Documentation
