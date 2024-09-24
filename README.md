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
```


## How It Works
The recommender system is based on content similarity between movies. The steps are as follows:

1. **Data Preprocessing**: The dataset is cleaned and necessary features like genres, keywords, and descriptions are extracted and processed.
2. **Feature Vectorization**: The TF-IDF (Term Frequency-Inverse Document Frequency) vectorizer converts the textual data into vectors.
3. **Cosine Similarity Calculation**: Cosine similarity is used to measure how similar two movies are based on their feature vectors.
4. **Recommendation Engine**: Given a movie title, the system computes similarity scores with other movies and recommends the top N similar movies.

## Dataset
The dataset used for this project is from [TMDb (The Movie Database)](https://www.themoviedb.org/). It contains information such as:
- Movie titles
- Genres
- Keywords
- Overview/Description
- Cast and Crew details

## Installation and Setup

### Prerequisites
Make sure you have the following installed:
- Python 3.7+
- pip (Python package installer)

### Clone the Repository
```bash
git clone https://github.com/your-username/movie-recommender-system-tmdb-dataset.git
cd movie-recommender-system-tmdb-dataset
```

### Install Dependencies
Install the required libraries from `requirements.txt`:
```bash
pip install -r requirements.txt
```

### Run the Streamlit Application
To launch the web app using Streamlit, run the following command:
```bash
streamlit run app.py
```
### Key Libraries Used
Pandas: For data manipulation and cleaning.
Scikit-learn: For feature vectorization (TF-IDF) and similarity calculation.
Streamlit: For building the interactive web app.
Numpy: For numerical operations.
