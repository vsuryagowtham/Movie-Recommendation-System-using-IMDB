# Movie-Recommendation-System
## Overview
This project implements a content-based movie recommender system using the TMDb dataset. The system utilizes cosine similarity to recommend movies based on features like genre, keywords, and descriptions. The project is developed using Python and deployed as an interactive web application via Streamlit.

## Features
- **Content-Based Recommendations**: Recommend movies based on their genre, keywords, and descriptions.
- **Cosine Similarity**: Calculates similarity between movies using cosine similarity based on their feature vectors.
- **Streamlit Interface**: Provides an easy-to-use interface for users to input their favorite movies and get recommendations.
- **Efficient Data Handling**: The project uses Pandas for data manipulation and TF-IDF for text feature extraction.

## Project Structure
```bash
Movie-Recommender-System/
│
├── recommender.ipynb        # Jupyter notebook for the recommendation logic
├── data/                    # Folder containing the TMDb dataset
│   └── tmdb_movies.csv      # Dataset file with movie information
├── app.py                   # Streamlit application code for deployment
├── README.md                # Project documentation
└── requirements.txt         # List of dependencies

