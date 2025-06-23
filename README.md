# Trader Performance vs Market Sentiment

This project investigates the relationship between individual trader performance and crypto market sentiment, using historical trading data and the Bitcoin Fear & Greed Index.

## Project Overview

- Objective: Analyze whether market sentiment (Fear, Neutral, Greed) has an impact on trader profitability.
- Sentiment Data Source: Alternative.me's Bitcoin Fear & Greed Index.
- Trade Data Source: Hyperliquid historical trader dataset.
- Outcome: Generate actionable insights and visualizations that help understand how traders perform under varying market emotions.

## Datasets Used

| Dataset                  | Description                                                       |
|--------------------------|-------------------------------------------------------------------|
| `historical_data.csv`    | Contains trading activity including timestamps, execution prices, side, size, closed PnL, and leverage. |
| `fear_greed_index.csv`   | Daily market sentiment values and classifications (Fear, Greed, etc). |

## Tools and Technologies

- Python (Pandas, Matplotlib, Seaborn)
- Jupyter Notebook
- Git and GitHub

## Analysis Performed

- Cleaned and preprocessed both datasets.
- Merged datasets on date fields to align sentiment with trading activity.
- Calculated average and median PnL for each sentiment classification.
- Computed win/loss ratios under different sentiment conditions.
- Visualized key trends and relationships using bar plots and summary tables.

## Key Insights

- Trader profitability varies significantly based on market sentiment.
- Certain sentiment conditions (e.g., Fear or Greed) correspond with more frequent or higher-value wins/losses.
- These patterns can inform smarter, sentiment-aware trading strategies.

## Folder Structure

```
project-root/
├── data/                   # Contains historical_data.csv and fear_greed_index.csv
├── notebooks/              # Jupyter notebooks with analysis
├── output/                 # Generated charts and CSV summaries
├── requirements.txt        # Python dependencies
└── README.md               # Project documentation
```

## How to Run

1. Clone the repository:
   ```
   git clone https://github.com/your-username/trader-performance-vs-market-sentiment.git
   ```

2. Navigate into the project directory:
   ```
   cd trader-performance-vs-market-sentiment
   ```

3. Create and activate a virtual environment:
   ```
   python -m venv env
   source env/bin/activate   # On Windows: env\Scripts\activate
   ```

4. Install dependencies:
   ```
   pip install -r requirements.txt
   ```

5. Open the Jupyter notebook and run the analysis:
   ```
   jupyter notebook
   ```
