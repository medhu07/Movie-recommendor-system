# Movie Recommender System

This project is a movie recommender system built using machine learning techniques such as content-based filtering. It suggests movies similar to a user's input based on metadata like genres, keywords, cast, and crew.

## Dataset

The system is powered by the **TMDB 5000 Movies and Credits Dataset**, which includes:

- `tmdb_5000_movies.csv`: Contains metadata about 5000 movies (genres, keywords, overview, etc.)
- `tmdb_5000_credits.csv`: Contains cast and crew information for those movies

Dataset source: [Kaggle - TMDB 5000 Movie Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)

## Features

- Content-based movie recommendations
- Uses metadata such as:
  - Genres
  - Keywords
  - Cast
  - Crew
  - Movie overviews
- Fast similarity search using cosine similarity on vectorized features

## How It Works

1. The metadata from both files is merged into a single dataset.
2. Key features are extracted and combined into a single string (tags).
3. Text data is vectorized using `CountVectorizer`.
4. Cosine similarity is calculated between all movie vectors.
5. Given a movie title, the system recommends the most similar movies.

## Installation

Clone the repo:

```bash
git clone https://github.com/yourusername/movie-recommender.git
cd movie-recommender
