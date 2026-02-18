# Spotify Music Insights — PostgreSQL Data Analysis

In this project, I analyzed Spotify track-level data using PostgreSQL to explore genre representation, artist popularity, and audio feature trends. My objective was to understand how musical attributes such as energy, danceability, acousticness, valence, and tempo correlate with song popularity and genre classification.

Through structured SQL analysis, I evaluated how different musical characteristics influence listener engagement and how genres differ in their overall audio profiles. This project simulates how streaming platforms might use audio data to refine recommendation systems and playlist strategies.

## Project Objectives
In this analysis, I aimed to answer the following business questions:
In this analysis, I aimed to answer the following business questions:
1. How many songs are classified under each genre?
2. Which artist has the highest average popularity across their songs?
3. What is the average energy level for songs longer than 3 minutes?
4. Which songs have both high danceability and high valence?
5. How many songs have loudness levels below -10 dB?
6. What is the average speechiness value per genre?
7. What’s the shortest and longest song length in the dataset?
8. Which genres have the highest average acousticness?
9. How does popularity differ between songs with high vs. low liveness?
10. Which artist appears most frequently in the dataset?
11. How many songs have a popularity score above 80?
12. Which genres tend to have lower valence (more melancholic)?
13. What is the average BPM (tempo) for each genre?

## Tools & Technical Approach
In this project, I used:
- PostgreSQL
- Aggregate functions (COUNT, AVG, MIN, MAX) for genre and feature analysis
-GROUP BY and ORDER BY for ranking and segmentation
- CASE statements to categorize high vs. low feature thresholds
- FILTER clauses for conditional aggregations
- Numeric comparisons to segment audio feature intensity levels
- Time-based calculations to evaluate song duration

I structured queries to compare audio feature distributions across genres and identify correlations between musical characteristics and popularity scores.

## Key Insights / Results
Through this analysis, I identified:
- Pop, rap, and EDM are among the most represented genres in the dataset.
- One artist stands out with the highest average popularity, indicating consistent engagement across their tracks.
- Songs longer than three minutes tend to maintain relatively high energy levels, aligning with mainstream radio and live performance standards.
- Tracks with both high danceability and high valence are generally upbeat and playlist-friendly.
- Genres such as folk and singer-songwriter rank highest in acousticness, reflecting lower electronic production.
- Songs with lower liveness values show slightly higher average popularity, suggesting studio-produced tracks may perform better commercially.
- Certain genres consistently display lower valence scores, reflecting more introspective or emotional themes.
- Techno and house music maintain higher average BPM values, aligning with energetic club environments.

This analysis demonstrates how audio feature data can be leveraged to support recommendation engines, playlist curation, artist marketing strategy, and audience segmentation.

## What I Learned
Through this project, I strengthened my ability to:
- Analyze numeric feature distributions in SQL
- Compare genre-level aggregates across multiple audio dimensions
- Segment data using threshold-based logic
- Interpret correlations between content characteristics and popularity
- Translate music metadata into product and marketing insights

I also gained practical insight into how streaming platforms might optimize content exposure based on measurable audio features.

## Challenges I Encountered

One challenge I faced was defining meaningful thresholds for “high” vs. “low” audio features (e.g., danceability or valence). I addressed this by using consistent benchmark ranges and validating distributions before segmentation.

Another challenge involved comparing genres with vastly different representation sizes, which required careful aggregation to avoid skewed interpretations.

Additionally, interpreting feature correlations required caution to avoid assuming causation without deeper statistical modeling.


## Dataset Overview
The Spotify dataset contains track-level audio features and metadata, including:
- Genre, Artist Name, Track Title
- Popularity Score
- Energy, Danceability, Acousticness, Valence
- Liveness, Speechiness, Loudness, Tempo
- Song Length (seconds) and Beats Per Minute (BPM)
