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
  recommendations('Toy Story (1995)')
  1815                                           Antz (1998)
2496                                    Toy Story 2 (1999)
2967        Adventures of Rocky and Bullwinkle, The (2000)
3166                      Emperor's New Groove, The (2000)
3811                                 Monsters, Inc. (2001)
6617     DuckTales: The Movie - Treasure of the Lost La...
6997                                      Wild, The (2006)
7382                                Shrek the Third (2007)
7987                        Tale of Despereaux, The (2008)
9215     Asterix and the Vikings (Astérix et les Viking...
9732                                          Turbo (2013)
10052                                Boxtrolls, The (2014)
1595                            Black Cauldron, The (1985)
1675                         Lord of the Rings, The (1978)
2696                 We're Back! A Dinosaur's Story (1993)
3420                      Atlantis: The Lost Empire (2001)
3535                          Land Before Time, The (1988)
4314     Pokemon 4 Ever (a.k.a. Pokémon 4: The Movie) (...
4799               Sinbad: Legend of the Seven Seas (2003)
5539                         Phantom Tollbooth, The (1970)
Name: title, dtype: object

    ```
