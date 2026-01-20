Music Recommendation System (Content-Based/Artist-based)

Overview:
This project implements a content-based music recommendation system that suggests songs similar to a given track using cosine similarity over numerical song features. The system focuses on correctness, explicit self-similarity removal, and proper evaluation against a random baseline.

Features:
Content-based filtering using audio and metadata features
Cosine similarity for measuring song-to-song similarity
Explicit removal of self-recommendations
Random baseline comparison for validation
Leave-one-out evaluation strategy

Technologies Used:
Python
Pandas
NumPy
Scikit-learn
Jupyter Notebook

How It Works:
Each song is represented as a numerical feature vector
Cosine similarity is computed between a query song and all songs
Top-k most similar songs are selected (excluding the query song)
Recommendations are evaluated against randomly selected songs

Evaluation Method:
To validate recommendation quality, the system compares:
Average cosine similarity of model recommendations
Average cosine similarity of random recommendations (baseline)
A higher similarity score for the model confirms meaningful recommendations.

Key Design Choices:
Explicit removal of self-similarity to prevent inflated scores
Defensive handling of indices and edge cases
Baseline comparison instead of misleading accuracy metrics

dataset link:
https://www.kaggle.com/datasets/zaheenhamidani/ultimate-spotify-tracks-db/data
