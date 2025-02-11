# Binance Trading Volume Analyzer

## Overview
This Jupyter Notebook fetches real-time trading volume data from Binance and analyzes it using OpenAI's GPT-based financial assistant. The data is collected, stored as CSV files with timestamps, and processed for insights into market trends.

## Features
- Fetches live trading volume data from Binance API
- Stores trading volume data in timestamped CSV files
- Uploads and analyzes the data using OpenAI's assistant
- Provides market insights, trends, and potential trading strategies

## Requirements

### Dependencies
Ensure you have the following Python packages installed:
```sh
pip install binance pandas tqdm openai
```

### API Keys
This notebook requires Binance API keys and OpenAI API credentials. Store them in a `config.py` file as:
```python
# config.py
class myconfig:
    BINANCE_API_KEY = "your_binance_api_key"
    BINANCE_API_SECRET = "your_binance_api_secret"
    OPENAI_API_KEY = "your_openai_api_key"
    OPENAI_ORG = "your_openai_organization"
    OPENAI_PROJECT = "your_openai_project"
```

## Usage

### 1. Fetch Binance Trading Data
Run each cell sequentially in the Jupyter Notebook to collect and save trading volume data.

### 2. Upload Data and Analyze
The notebook automatically:
- Uploads the generated CSV file to OpenAI
- Uses OpenAI's assistant to analyze market trends
- Outputs insights regarding market movement, fluctuations, and potential trading strategies

## Output
- A timestamped CSV file containing trading volume details
- AI-generated market analysis displayed within the notebook

## Example Output
```
Fetching trading volume: 100%|███████████████████████████████| 500/500 [00:30<00:00, 16.5 pairs/s]
Data successfully saved to data/binance_trading_volume_2025-02-11_15-01-43.csv

Market Analysis Report:
1. Market is showing an overall upward trend...
2. Notable fluctuations detected in BTCUSDT and ETHUSDT...
3. Potential trading strategies include...
```

## Notes
- Ensure your Binance API keys have read permissions.
- OpenAI API usage may incur costs; monitor your OpenAI account.

## License
This project is open-source. Feel free to modify and improve!

