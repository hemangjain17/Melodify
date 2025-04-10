🎶 Melodify - AI-Powered Music Recommender System
Melodify is an AI-driven content-based music recommender system designed to enhance music discovery through personalized song suggestions. It analyzes lyrics, artist attributes, and song features to generate accurate similarity scores between tracks, helping users explore music tailored to their tastes.

🚀 Features
Personalized Song Recommendations based on previously liked tracks.

Content-Based Filtering using audio features, lyrics, and artist metadata.

Multilingual Lyrics Support powered by XLM-RoBERTa for cross-language embedding.

Rich Song Metadata including popularity, duration, danceability, energy, and more.

Artist Profiling through BERT embeddings, artist genres, and popularity.

Custom Similarity Scoring Engine using cosine similarity, inverse Manhattan distance, and feature weighting.

Data Visualization and feature transformation for improved model performance.

Lyric Insights using text embeddings for emotional and thematic analysis.

25K+ Songs Dataset with complete metadata from Spotify and lyrics scraped using multiple APIs and fallback scrapers.

🧠 Technology Stack
Python, Pandas, NumPy, scikit-learn

Spotify Web API, YTMusic API, Musixmatch, Tekstowo (for lyrics)

XLM-RoBERTa, BERT Uncased, Sentence Transformers

BeautifulSoup, Selenium

Matplotlib, Seaborn (for visualizations)

📂 Feature Categories
🎵 Song Features
Name, Duration, Popularity, Explicit flag

Tempo, Danceability, Acousticness, Valence

Key, Mode, Energy, Loudness, Speechiness

📝 Lyrics Embedding
Collected and processed via XLM-RoBERTa for multilingual accuracy

👨‍🎤 Artist Features
Artist and Album embeddings

Artist genres, popularity, and follower count

🌍 Language Detection
One-hot encoded languages to enhance culturally relevant recommendations

🔍 Recommendation Logic
Preprocess metadata and embeddings (lyrics, artist, and song features).

Assign weights to features based on their relevance.

Flatten all features into a weighted vector space.

Calculate similarity scores using:

Cosine Similarity

Inverse Manhattan Distance

Equality Checks

Recommend top-N most similar songs based on the final aggregated similarity score.

✅ Results
High accuracy based on similarity threshold scoring.

Human testing validates logical grouping of genres, moods, and energy levels.

Successfully identified and recommended songs in different languages and genres.

⚠️ Challenges Faced
Limitations in API access (especially for lyrics).

Scraping constraints on various platforms.

Handling multilingual data with inconsistent formatting.

Audio feature redundancies and data cleaning complexities.
