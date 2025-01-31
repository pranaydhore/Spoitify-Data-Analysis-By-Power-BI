<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Spotify Analysis Project - Power BI & DAX</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 40px;
            padding: 20px;
            background-color: #f4f4f4;
        }
        .container {
            max-width: 800px;
            margin: auto;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        h1 {
            text-align: center;
            color: #1DB954;
        }
        .poster {
            text-align: center;
            margin: 20px 0;
        }
        img {
            max-width: 100%;
            border-radius: 10px;
        }
        .keypoints {
            padding: 10px;
            background: #e0ffe0;
            border-left: 5px solid #1DB954;
        }
        .dax-code {
            background: black;
            color: limegreen;
            padding: 10px;
            border-radius: 5px;
            font-family: monospace;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        .animated {
            animation: fadeIn 2s ease-in;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Spotify Analysis Project 🎵📊</h1>
        <div class="poster animated">
<!--             <img src="spotify_poster.jpg" alt="Spotify Project Poster"> -->
        </div>
        <h2>📌 Key Points</h2>
        <div class="keypoints">
            <ul>
                <li>Analyzing Spotify streaming data using Power BI</li>
                <li>Using DAX formulas to derive insights</li>
                <li>Creating interactive dashboards</li>
                <li>Finding trends in songs, artists, and genres</li>
                <li>Understanding user behavior and popular playlists</li>
                <li>Comparing music trends across different countries</li>
                <li>Understanding seasonal impacts on music streaming</li>
                <li>Analyzing the rise of independent artists</li>
                <li>Discovering emerging music genres</li>
                <li>Utilizing AI and ML in music trend predictions</li>
            </ul>
        </div>
        <h2>🖩 DAX Formulas Used</h2>
        <pre class="dax-code">
Total Streams = SUM(SpotifyData[Streams])
Top Artist = CALCULATE(MAX(SpotifyData[Artist]), FILTER(SpotifyData, SpotifyData[Streams] = MAX(SpotifyData[Streams])))
Top Genre = CALCULATE(MAX(SpotifyData[Genre]), FILTER(SpotifyData, SpotifyData[Streams] = MAX(SpotifyData[Streams])))
Average Streams per Artist = AVERAGEX(VALUES(SpotifyData[Artist]), SUM(SpotifyData[Streams]))
Top Song by Popularity = CALCULATE(MAX(SpotifyData[Song]), FILTER(SpotifyData, SpotifyData[Popularity] = MAX(SpotifyData[Popularity])))
        </pre>
        <h2>📖 Theory & Insights</h2>
        <p>Spotify's dataset allows us to explore music trends, user preferences, and song popularity. Using Power BI, we can create dynamic reports that help identify:</p>
        <ul>
            <li>Most streamed songs and artists</li>
            <li>Genre preferences by country</li>
            <li>Seasonal trends in music consumption</li>
            <li>Impact of playlists on song popularity</li>
            <li>Correlation between song features (tempo, loudness, energy) and popularity</li>
            <li>Growth of independent artists compared to record label artists</li>
            <li>Identifying breakout songs and viral trends</li>
            <li>Analyzing playlist curation strategies</li>
        </ul>
        <h2>🎼 Data Sources & Collection</h2>
        <p>Spotify's dataset can be accessed using various APIs, web scraping, or publicly available data from Kaggle. The dataset generally includes:</p>
        <ul>
            <li>Song title, artist, album</li>
            <li>Genre, release year</li>
            <li>Number of streams</li>
            <li>Popularity ranking</li>
            <li>Audio features such as danceability, tempo, energy, loudness</li>
        </ul>
        <h2>📊 Power BI Dashboard Features</h2>
        <ul>
            <li>Interactive visualizations of top artists and genres</li>
            <li>Time-series analysis of music trends</li>
            <li>Custom filters for user exploration</li>
            <li>Comparison of different music streaming behaviors across regions</li>
        </ul>
        <h2>🚀 Conclusion</h2>
        <p>With Power BI and DAX, we can uncover deep insights into the world of music streaming, providing valuable information for artists, record labels, and marketers. This project helps in understanding what makes a song popular and how music trends evolve over time.</p>
    </div>
</body>
</html>
