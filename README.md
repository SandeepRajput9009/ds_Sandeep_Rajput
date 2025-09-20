# Project: Bitcoin Sentiment & Trader Performance

This project explores the relationship between Bitcoin market sentiment and trader performance using two primary datasets: the Bitcoin Market Sentiment Dataset (tracking Fear and Greed indices) and Historical Trader Data from Hyperliquid (including trade details, PnL, leverage, and more). By analyzing these datasets together, the project aims to uncover hidden patterns, identify factors influencing trader success, and provide actionable insights to inform smarter trading strategies in the crypto market.

## 📂 Folder Structure

##  How to Run
1. Open `notebook_1.ipynb` in **Google Colab**.  
   - Link: [Colab Notebook](https://colab.research.google.com/) (replace with your shared link).  
   - Ensure **Anyone with the link can view** is enabled.
2. Upload the two raw datasets:
   - `fear_greed_index.csv` (sentiment dataset)  
   - `historical_data.csv` (trader dataset)
3. Run all cells sequentially.  
   - Data will be cleaned, merged, and analyzed.  
   - Intermediate CSVs are saved in `csv_files/`.  
   - Plots are saved in `outputs/`.

##  Key Outputs
- **CSV Files**: Aggregated account- and platform-level metrics.  
- **Charts**:  
  - Histogram of daily PnL  
  - Boxplot of daily PnL by sentiment (Fear vs Greed)  
  - Platform total PnL timeseries  
- **Report**: `ds_report.pdf` with insights & recommendations.

## Requirements
- Google Colab (Python 3 environment)  
- Python libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`, `xgboost` (if running modeling part)

## Notes
- All timestamps were normalized to **IST** for daily aggregation.  
- Sentiment classification: `Fear=0`, `Greed=1`.  
- If numeric sentiment index is available, it is used in correlation & event studies.  
