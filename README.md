# Movie Recommendation System

## Overview
This project is a movie recommendation system that suggests movies to users based on their input. It processes movie data, cleans it, and utilizes machine learning techniques to provide personalized recommendations.

## Libraries Used
- `pandas`: For data manipulation and analysis.
- `matplotlib`: For plotting and visualization.
- `wordcloud`: For generating word clouds.
- `sklearn` (scikit-learn): For machine learning algorithms and tools.

## Features
- Data cleaning and visualization.
- Generation of word clouds for visualizing movie genres and descriptions.
- TF-IDF vectorization to convert text data into meaningful numerical representations.
- Calculation of similarities between movies using linear kernel functions.

## Usage

1. Import the necessary libraries:
    ```python
    import pandas as pd
    import matplotlib.pyplot as plt
    from wordcloud import WordCloud
    from sklearn.feature_extraction.text import TfidfVectorizer
    from sklearn.metrics.pairwise import linear_kernel
    2. Load and clean your dataset:
    ```python

    # Load the dataset
    movies = pd.read_csv('path_to_your_movie_dataset.csv')
    
    # Clean the data (example: remove null values, duplicates, etc.)
    movies = movies.dropna().drop_duplicates()
    
    # Show the cleaned data
    print(movies.head())

  # Output
You can type in the name of a movie and the system will output a list of recommended movies based on the similarity scores
    ```
