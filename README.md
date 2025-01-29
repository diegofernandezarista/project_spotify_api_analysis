# Spotify API Analysis: Unveiling Trends in 2024 Music Releases 🎶🎧

## Overview 🚀  
Welcome to Spotify API Analysis! This project explores trends in song and album popularity for 2024 releases on Spotify. Using data pulled from the Spotify API, we analyze how factors such as song duration, release timing, track count, featured artists, and artist followers influence streaming success.  
If you're curious about what makes an album or song a hit, this analysis provides data-backed insights into the music industry's evolving landscape.

## Data Collection Methodology 🌐  
Data was collected via the Spotify API using the Spotipy library, focusing on albums, songs, and artists from 2024 releases. The retrieved data includes:  

- Album details (e.g., track count, popularity)  
- Song-level data (e.g., track popularity, duration, featured artists)  
- Artist information (e.g., number of followers, genres)  

All data is stored in pickle (.pkl) files for ease of use. If you want to replicate the analysis, simply load the provided .pkl files instead of making API calls!

## Key Findings & Insights 🎶🎧  

### 🔍 Statistical Analysis of Popularity
- **Albums with more tracks** than the median are significantly more popular.  
- **Albums with more featured artists** show higher popularity.  

### 🌐 Artist Influence on Popularity
- **Artists with more followers release more successful albums**, though it's not the sole determining factor.  

### 🎵 Genre-Specific Trends
- **Afrobeats & Dancehall**: Strong link between artist followers and popularity.  
- **Latin Trap & Urbano Latino**: Fanbase is the most critical factor.  
- **Punjabi & Hindi Music**: Album length is a major success factor.   

## Limitations & Considerations ⚠️  

This analysis provides valuable insights but has some limitations:  

- Spotify API Limitations: Only 1,000 albums per year can be retrieved, affecting data completeness.  
- Album-only Focus: Singles and EPs are not included, though they may also impact industry trends.  
- Genre Classification: Genres are assigned to artists rather than individual albums, limiting genre-based analysis.  
- Statistical Assumptions: Tests assume normality and equal variance, which may not always hold.  

## Getting Started 🛠️  

### 1. Clone the repository:

```bash
git clone https://github.com/diegofernandezarista/project_spotify_api_analysis.git
cd project_spotify_api_analysis
```
### 2. Load Data for Analysis:
```python
import pickle
with open('pkl_file.pkl', 'rb') as f:
    data = pickle.load(f)
```
### 3. Run the Jupyter Notebook:
```bash
jupyter notebook
```

## Future Improvements ✨  

- Expand data collection methods to capture more than 1,000 albums per year for a more comprehensive dataset.
- Incorporate singles and EPs to provide a fuller picture of streaming trends and listener preferences.
- Dive deeper into genre analysis by overcoming the limitations of Spotify’s genre assignments to enhance accuracy.
- Develop machine learning models to predict album popularity based on historical trends and insights.

## Acknowledgments 🙏  

Special thanks to Spotipy for providing a Python client that simplifies access to the Spotify API, and to Spotify for Developers for granting API access, making this analysis possible!

If you’d like to discuss or collaborate on future enhancements, feel free to reach out!

Happy analyzing! 🎶🚀
