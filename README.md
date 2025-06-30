# **YouTube & Spotify Data Analysis 📊**
This on-going project is a personal data analysis tool that explores patterns and trends in my **Spotify streaming history** and **YouTube watch history**. The data was exported from **Google Takeout** and **Spotify's streaming history export**, and processed using Python, pandas, and SQL to uncover insights such as watch/listen frequency by hour, day, artist, and more.

⚠️ *Note: This project is based on personal and private data. The dataset is not included in the repository for privacy reasons.*

## **Key Features**
**📺 YouTube Watch History**
- Cleans and processes exported `watch-history.json`
- Converts timestamp data to local time and extracts:
    -  Hour, day of the week, month, and year
- Visualizes:
    - Watch frequency by hour, weekday, and year
    - Weekly/monthly viewing trends using time series line charts
- Structures data for relational database:
    - Watch history and channels

**🎧 Spotify Streaming History**
- Cleans and processes exported `Streaming_History_Audio.json`
- Converts timestamp data to local time and extracts:
    -  Hour, day of the week, month, and year
- Visualizes:
    - Top artists, songs, albums
    - Hourly and weekly listening behaviors
- Structures data for relational database:
    - streams, artists, albums, and songs

**🗃️ Database Integration**
- SQLite + SQLAlchemy used to:
    - Save cleaned data to .db file
    - Preparation for future SQL querying and relational joins

## **Directory Structure**
```
YouTube Data Analysis/
├── data/                # YouTube and Spotify data files are here
├── .gitignore           # Files and directories excluded from Git tracking
├── README.md            # Project documentation
├── requirements.txt     # Python dependencies
├── sptfy_analysis.ipynb # Spotify Data Analysis
└── yt_analysis.ipynb    # YouTube Data Analysis
```

## **Technologies Used**
- **Python 3** – Core language
- **pandas** – Data cleaning and manipulation
- **plotly / matplotlib** – Visualizations
- **sqlite3 / SQLAlchemy** – Database storage

## **Future Plans**
- Expand SQL-based querying on both datasets
- Add markdowns for insights
- Build an interactive dashboard
- Update for easier usage for other people

## **Getting Started with Your Own Data**
1. Export your data from **Google Takeout**
2. Export your Spotify data from [Spotify Privacy Settings](https://www.spotify.com/us/account/privacy/)
2. Place `.json` files into a `data/` folder
3. Check out `.ipynb` files to clean and explore your own data

## **Privacy and Security**
- Personal data is kept private and excluded via .gitignore
- All scripts operate on **local data** only. Users are responsible for securing their own data.
- This project is for local, personal use only