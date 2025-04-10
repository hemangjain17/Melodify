# 🎶 Melodify - AI-Powered Music Recommender System

**Melodify** is an AI-driven content-based music recommender system designed to enhance music discovery through personalized song suggestions. It analyzes lyrics, artist attributes, and song features to generate accurate similarity scores between tracks, helping users explore music tailored to their tastes.

---

## 🚀 Features

- **Personalized Song Recommendations** based on previously liked tracks.
- **Content-Based Filtering** using audio features, lyrics, and artist metadata.
- **Multilingual Lyrics Support** powered by **XLM-RoBERTa** for cross-language embedding.
- **Rich Song Metadata** including popularity, duration, danceability, energy, and more.
- **Artist Profiling** through BERT embeddings, artist genres, and popularity.
- **Custom Similarity Scoring Engine** using cosine similarity, inverse Manhattan distance, and feature weighting.
- **Data Visualization** and feature transformation for improved model performance.
- **Lyric Insights** using text embeddings for emotional and thematic analysis.
- **25K+ Songs Dataset** with complete metadata from Spotify and lyrics scraped using multiple APIs and fallback scrapers.

---

## 🧠 Technology Stack

- **Languages & Libraries**: Python, Pandas, NumPy, scikit-learn
- **APIs**: Spotify Web API, YTMusic API, Musixmatch, Tekstowo
- **Embeddings**: XLM-RoBERTa, BERT Uncased, Sentence Transformers
- **Web Scraping**: BeautifulSoup, Selenium
- **Visualization**: Matplotlib, Seaborn

---

## 📂 Feature Categories

### 🎵 Song Features
- Name, Duration, Popularity, Explicit flag
- Tempo, Danceability, Acousticness, Valence
- Key, Mode, Energy, Loudness, Speechiness

### 📝 Lyrics Embedding
- Collected and processed using **XLM-RoBERTa** for robust multilingual support.

### 👨‍🎤 Artist Features
- Artist and Album embeddings
- Genres, Popularity Score, Followers count

### 🌍 Language Detection
- One-hot encoded language features for better multilingual matching.

---

## 🔍 Recommendation Logic

1. Preprocess metadata and generate embeddings.
2. Apply manually defined weights to each feature group.
3. Flatten feature vectors and compute similarity using:
   - Cosine Similarity
   - Inverse Manhattan Distance
   - Equality Check
4. Return top-N most similar tracks based on the aggregated similarity score.

---

## ✅ Results

- High similarity scores across genres and artists.
- Threshold-based accuracy validated through human testing.
- Successfully handles multilingual and cross-genre recommendations.

---

## ⚠️ Challenges Faced

- API limitations, especially for lyrics access.
- Inconsistent data formats and scraping restrictions.
- Handling duplicate tracks and varying metadata quality.
- Data cleaning complexities for multilingual lyrics.


