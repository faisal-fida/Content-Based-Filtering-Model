# Content-Based Filtering Model

This project implements a content-based filtering model for recommending movies. The model uses various features extracted from a dataset of the top 1000 movies from IMDb to compute similarities and recommend similar movies.

## Overview

The goal of this project is to recommend movies based on their content. The key features considered include:

- **Overview**: The movie's plot summary.
- **Director**: The director of the movie.
- **Stars**: The main actors in the movie.
- **Gross**: The gross revenue of the movie.
- **IMDB Rating**: The rating of the movie on IMDb.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/faisal-fida/Content-Based-Filtering-Model.git
    ```
2. Install the required libraries:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Load the Jupyter Notebook `content-based filtering model.ipynb` in your Jupyter environment.
2. Run the notebook cells sequentially to preprocess the data, extract features, compute similarities, and make movie recommendations.
3. Use the `recommend_movies` function to get movie recommendations based on a given movie title.

## Challenges and Solutions

- **Data Cleaning**: Missing values in the dataset were filled or removed to ensure data consistency.
- **Feature Extraction**: Various features were one-hot encoded and normalized to be used in the similarity computation.
- **Similarity Computation**: Cosine similarity was used to compute the similarity between movies based on the extracted features.

## Example

Here is an example of how to get movie recommendations:

```python
movie_title = 'Pulp Fiction'
recommend_movies(movie_title, n=5)
```

Output:
```
['Brokeback Mountain', 'Forrest Gump', 'Naked', 'The Green Mile']
```

## Conclusion

This content-based filtering model provides a straightforward way to recommend movies based on their content. By leveraging various features and computing similarities, the model can successfully recommend movies that are similar to a given movie.

For more details, please refer to the Jupyter Notebook in this repository.
