## Movie/TV Show Recommendation System

This repository contains two Jupyter notebooks that implement movie/TV show recommendation systems using different datasets and environments:

**1. Movie_Recommendation_System.ipynb**

This notebook, created on Google Colab, utilizes a movie dataset sourced from Kaggle. It follows these steps:

   - **Data Import:** Imports the movie dataset from Kaggle using appropriate libraries.
   - **Data Cleaning:** Performs cleaning operations on the data to ensure its quality for analysis. This might include handling missing values, removing irrelevant columns, or formatting data types.
   - **Feature Identification:** Identifies the most important columns that might influence recommendation outcomes (e.g., title, genre, director, actors, synopsis).
   - **Feature Engineering:** Creates a new input column by concatenating the identified features into a single string. This string will be used to represent each movie/TV show for recommendation purposes.
   - **TF-IDF Vectorization:** Applies TF-IDF (Term Frequency-Inverse Document Frequency) vectorization using `TfidfVectorizer` from scikit-learn. This technique helps capture the importance of words within the input text. Experiments are conducted to determine the optimal `max_features` parameter, which in this case is set to 5000.
   - **Cosine Similarity:** Calculates cosine similarity between the user's input and each movie/TV show in the vectorized space. Cosine similarity measures how similar two documents are based on the angle between their vector representations.
   - **Recommendation Generation:** Sorts the movies/TV shows based on their cosine similarity scores in descending order. The top 10 most similar items are presented as recommendations for the user.

**2. [Netflix Recommendation.ipynb](https://www.kaggle.com/code/atharva729/netflix-recommendation)**

This notebook, created within the Kaggle notebook environment, uses a Netflix dataset sourced from Kaggle. It performs a similar process to `movie-recommendation.ipynb`:

   - Data import, cleaning, and feature engineering steps are likely analogous to the previous notebook, but tailored to the specific structure of the Netflix dataset.
   - TF-IDF vectorization and cosine similarity calculations are applied in the same manner as described previously.

**How to Use:**

1. Clone this repository: `git clone https://github.com/<your-username>/movie-tv-recommendation`
2. Navigate to the repository directory: `cd movie-tv-recommendation`
3. Install any required libraries using your preferred package manager (e.g., `pip install <library-name>`).
4. Open and run each Jupyter notebook (e.g., `jupyter notebook movie-recommendation.ipynb`).

The link to the kaggle notebook for the netflix recommendation file:
[Netflix Recommendation](https://www.kaggle.com/code/atharva729/netflix-recommendation)
