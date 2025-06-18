# **YouTube Watch History Analysis 📊**
This project is a personal data analysis and forecasting tool that explores patterns and trends in my YouTube watch history. The data was exported from **Google Takeout** and processed using Python and pandas to uncover information such as watch frequency by hour, day of the week, and trends across months and years. It also shows a time series forecasting, and saves the cleaned dataframe as a database file.

⚠️ Note: This project is based on personal and private data. The dataset is not included in the repository for privacy reasons.

## **Key Features**
- Cleans and processes exported `watch-history.json`
- Converts timestamp data to local time and extracts:
    -  Hour, day of the week, month, and year
- Visualizes:
    - Watch frequency by hour, weekday, and year
    - Weekly/monthly viewing trends using time series line charts
- Forecasting: 
    - Displays trend and seasonality patterns
    - Forecasts future watch activity using an ARIMA model
- Database Intergration:
    - Converts cleaned data into SQLite database

## **Directory Structure**
```
YouTube Data Analysis/
├── data/                # YouTube data files are here
├── .gitignore           # Files and directories excluded from Git tracking
├── README.md            # Project documentation
├── requirements.txt     # Python dependencies
└── yt_analysis.ipynb    # # Main script for cleaning, analyzing, visualizing
```

## **Future Plans**
- Full SQL database structure (MySQL or SQLite):
    - `watch_history`: timestamps, video titles, URLs
    - `channels`: frequency and metadata
- Add support for Spotify streaming history analysis
- Interactive dashboard

## **Technologies Used**
- **Python 3** – Core language
- **pandas** – Data cleaning and manipulation
- **plotly / matplotlib** – Visualizations
- **sqlite3 / SQLAlchemy** – Database storage and interaction
- **statsmodels** – Time series analysis and ARIMA modeling

## **Privacy and Security**
- `watch-history.json` contains sensitive personal data and is never shared.
- `.gitignore` protects private files in the `data/` folder.
- All scripts operate on **local data** only. Users are responsible for securing their own data.

## **Getting Started with Your Own Data**
1. Export your data from **Google Takeout**
2. Place `watch-history.json` inside a `data/` folder
3. Check out `yt_analysis.ipynb` to clean and explore your watch history

## **Notes**
- This project is for personal use and experimentation with Python and SQL.
- You can fork and replace with your own Takeout data to explore your habits.