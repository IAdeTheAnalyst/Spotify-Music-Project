# 🎵 Spotify Music Insights — PostgreSQL Data Analysis

This project analyzes Spotify song data to explore genre trends, artist popularity, and audio feature patterns. It provides actionable insights into how musical characteristics like energy, danceability, acousticness, and valence correlate with popularity and genre.

## 🧠 Key Business Questions
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

## 📊 Tools Used
- **SQL (PostgreSQL)**
- **Aggregate Functions**
- **FILTER Clause**
- **CASE Statements**
- **GROUP BY & ORDER BY**
- **MIN/MAX Aggregates**
- **Audio Feature Analysis (danceability, energy, liveness, valence, etc.)**

## 📌 Key Insights
- **Genre Distribution:** Pop, rap, and EDM are among the most represented genres in the dataset.
- **Artist Spotlight:** The artist with the highest average popularity stands out significantly, hinting at consistent fan engagement or strong marketing.
- **Energy & Length:** Songs longer than 3 minutes tend to maintain high energy levels—ideal for live performance or radio play.
- **Danceability & Mood:** Tracks with both high danceability and valence reflect upbeat, feel-good music—often prime candidates for playlists.
- **Acoustic Vibes:** Folk and singer-songwriter genres dominate the top of acousticness rankings, suggesting minimal electronic production.
- **Liveness & Popularity:** Songs with lower liveness values are slightly more popular, potentially due to cleaner studio production.
- **Sad Songs by Genre:** Certain genres consistently show low valence scores, suggesting they cater to more emotional or introspective themes.
- **Tempo Trends:** Genres like techno and house music maintain higher average BPMs, aligning with energetic club settings.

## 📂 Dataset Overview
The Spotify dataset includes a variety of track-level audio and metadata fields, such as:
- Genre, Artist Name, Track Title
- Popularity Score
- Energy, Danceability, Acousticness, Valence
- Liveness, Speechiness, Loudness, Tempo
- Song Length (seconds), Beats per Minute

> **Source:** [Spotify Tracks Dataset | Kaggle](https://www.kaggle.com/datasets)
