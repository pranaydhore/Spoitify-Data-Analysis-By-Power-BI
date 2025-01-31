# Spotify Data Analysis By Power BI 🎵📊

## 📌 Key Points
- Analyzing Spotify streaming data using Power BI
- Using DAX formulas to derive insights
- Creating interactive dashboards
- Finding trends in songs, artists, and genres
- Understanding user behavior and popular playlists
- Comparing music trends across different countries
- Understanding seasonal impacts on music streaming
- Analyzing the rise of independent artists
- Discovering emerging music genres
- Utilizing AI and ML in music trend predictions
- Identifying factors influencing song virality
- Understanding the role of collaborations in song success
- Exploring the impact of streaming algorithms on song popularity
- Examining user engagement based on listening habits

## 🖩 DAX Formulas Used
# DAX
Total Streams = SUM(SpotifyData[Streams])

Top Artist = CALCULATE(MAX(SpotifyData[Artist]), 
    FILTER(SpotifyData, SpotifyData[Streams] = MAX(SpotifyData[Streams])))

Top Genre = CALCULATE(MAX(SpotifyData[Genre]), 
    FILTER(SpotifyData, SpotifyData[Streams] = MAX(SpotifyData[Streams])))

Average Streams per Artist = AVERAGEX(VALUES(SpotifyData[Artist]), 
    SUM(SpotifyData[Streams]))

Top Song by Popularity = CALCULATE(MAX(SpotifyData[Song]), 
    FILTER(SpotifyData, SpotifyData[Popularity] = MAX(SpotifyData[Popularity])))

Monthly Growth Rate = (SUM(SpotifyData[Streams]) - 
    CALCULATE(SUM(SpotifyData[Streams]), PREVIOUSMONTH(SpotifyData[Date]))) / 
    CALCULATE(SUM(SpotifyData[Streams]), PREVIOUSMONTH(SpotifyData[Date]))


## 📖 Theory & Insights
Spotify's dataset allows us to explore music trends, user preferences, and song popularity. Using Power BI, we can create dynamic reports that help identify:
- Most streamed songs and artists
- Genre preferences by country
- Seasonal trends in music consumption
- Impact of playlists on song popularity
- Correlation between song features (tempo, loudness, energy) and popularity
- Growth of independent artists compared to record label artists
- Identifying breakout songs and viral trends
- Analyzing playlist curation strategies
- Examining the influence of music streaming platforms' recommendation algorithms
- Understanding the impact of collaborations between artists
- Investigating trends in streaming based on time of day and user demographics
- Analyzing the role of social media in boosting music streams

## 🎼 Data Sources & Collection
Spotify's dataset can be accessed using various APIs, web scraping, or publicly available data from Kaggle. The dataset generally includes:
- Song title, artist, album
- Genre, release year
- Number of streams
- Popularity ranking
- Audio features such as danceability, tempo, energy, loudness
- Playlist inclusion and recommendation frequency
- Listener engagement metrics (replays, skips, saves)

## 📊 Power BI Dashboard Features
- Interactive visualizations of top artists and genres
- Time-series analysis of music trends
- Custom filters for user exploration
- Comparison of different music streaming behaviors across regions
- Trend forecasting using machine learning techniques
- Playlist impact analysis on individual song growth
- Engagement rate analysis for different music categories
- Predictive analytics for upcoming hit songs

## 🚀 Conclusion
With Power BI and DAX, we can uncover deep insights into the world of music streaming, providing valuable information for artists, record labels, and marketers. This project helps in understanding what makes a song popular and how music trends evolve over time. By leveraging data analytics, we can predict future trends, optimize music recommendations, and enhance the overall listener experience.

---
**![Spotify Project Poster](Spotify.jpg)**
**![Spotify Project Poster](Spotify.jpg)**
**![Spotify Project Poster](Spotify.jpg)**
