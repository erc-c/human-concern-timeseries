Human Concern Timeseries 
A time series analysis of global search behavior patterns for five human concern 
indicators - Anxiety, Depression, Insomnia, Loneliness and Stress - using Google 
Trends data from January 2004 to March 2026.

Preview
![Anomaly Detection Dashboard](anomaly_detection.png)

Tools 
- Python · Pandas · Matplotlib · Seaborn · Statsmodels · Prophet
- Jupyter Notebook
- Power BI

Analysis Performed
- Data loading, cleaning and monthly resampling
- Multi-line trend visualization (2004-2026)
- Correlation analysis across all 5 concerns
- Seasonality heatmaps
- STL Decomposition (Trend · Seasonality · Residual)
- Z-Score Anomaly Detection
- 12-Month Rolling Standard Deviation (Volatility)
- Prophet Forecasting (2026-2028)

Key Findings
- Anxiety shows a clear sustained upward trend post-2015
- Loneliness recorded a sharp volatility spike in 2020, rising to 9.68
- Insomnia is projected to reach the highest relative search levels through 2028
- 55 anomaly spikes detected - Depression and Stress most frequently flagged
- 2025-2026 shows unprecedented simultaneous volatility across all 5 concerns

Power BI Dashboard
7 pages:
- Navigation
- Trend Lines
- Anomaly Detection
- Forecast
- Summary
- Temporal Patterns
- Volatility and Stability

Data Notes
- Source: Google Trends (trends.google.com)
- Each term downloaded separately - values are independently normalized to 0-100
- Monthly resolution across 267 data points (January 2004 - March 2026)
- 5 concerns tracked: Anxiety, Depression, Insomnia, Loneliness, Stress

Project Structure
```
├── Analysis.ipynb
├── anxiety.csv
├── depression.csv
├── insomnia.csv
├── loneliness.csv
├── stress.csv
├── outputs/
└── human-concern-timeseries.pbix
```
