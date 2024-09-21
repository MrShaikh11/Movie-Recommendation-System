# Movie Recommendation System

This project is a movie recommendation system built using Python, Pandas, Scikit-learn, and Jupyter widgets. It recommends similar movies based on user input and ratings data. The project is inspired by a tutorial from the [Dataquest YouTube channel](https://www.youtube.com/watch?v=eyEabQRBMQA).

## Features

- **Search Movies:** Users can search for a movie title, and the system will return the top 5 similar movie recommendations using a TF-IDF vectorizer and cosine similarity.
- **Recommend Similar Movies:** Based on user ratings, the system finds and recommends movies similar to those a user has liked (rated higher than 4).

## How It Works

1. **Data Preprocessing:**
    - The dataset contains movie titles and ratings.
    - The titles are cleaned using a regular expression to remove special characters.

2. **Text Vectorization:**
    - Titles are vectorized using the TF-IDF (Term Frequency-Inverse Document Frequency) method, considering both unigrams and bigrams.
    - Cosine similarity is computed to compare how similar different movie titles are.

3. **Movie Search:**
    - When the user inputs a movie title, the system returns the top 5 movies with the highest similarity scores.

4. **User-Based Recommendations:**
    - The system uses collaborative filtering to recommend movies by finding users with similar tastes (based on ratings) and suggesting movies that those users have rated highly.

## Installation

To run the project locally, follow these steps:

1. Clone the repository:
    ```bash
    git clone <repository-url>
    cd movie-recommendation-system
    ```

2. Install the necessary dependencies:
    ```bash
    pip install pandas scikit-learn ipywidgets
    ```

3. Run the Jupyter Notebook:
    ```bash
    jupyter notebook
    ```

## Usage

- Once the notebook is running, input the title of a movie into the search box, and the system will display similar movie recommendations.
- For personalized recommendations, the system suggests movies based on ratings provided by users similar to you.

## Technologies Used

- **Python:** Main programming language used in the project.
- **Pandas:** Used for data manipulation and analysis.
- **Scikit-learn:** For implementing the TF-IDF vectorizer and cosine similarity.
- **Jupyter Widgets (ipywidgets):** For interactive UI elements in the Jupyter Notebook.

## Acknowledgments

This project is based on the tutorial from the [Dataquest YouTube channel](https://www.youtube.com/watch?v=eyEabQRBMQA).

## License

This project is licensed under the MIT License.
