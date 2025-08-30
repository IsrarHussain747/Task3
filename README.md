🎬 Movie Recommendation System

📌 Project Overview

This project implements a hybrid movie recommendation system using both:

Content-Based Filtering – recommends movies similar to a given movie based on genres and tags.

Collaborative Filtering – recommends movies to a user based on ratings from similar users.

The system uses the MovieLens dataset (movies, ratings, tags) and demonstrates how recommendation engines work in practice.

🚀 Features

Load and preprocess movie, rating, and tag datasets

Parse genres and aggregate tags for feature engineering

Compute TF-IDF vectors of movie metadata for content similarity

Build a cosine similarity user-user matrix for collaborative filtering

Functions to:

Recommend similar movies (content-based)

Recommend movies for a given user (collaborative)

Example outputs for popular movies like Inception

📂 Dataset

The project uses the MovieLens dataset (CSV files):

movies.csv → movie titles, genres

ratings.csv → user ratings

tags.csv → user-generated tags

You can download it from MovieLens or use a Kaggle version.

🛠️ Technologies Used
Python 3

pandas – data handling

scikit-learn – TF-IDF, cosine similarity

difflib – fuzzy matching for titles

NumPy – matrix operations

⚙️ Installation
Clone the repository and install dependencies:

bash
Copy code
git clone https://github.com/your-username/movie-recommendation-system.git
cd movie-recommendation-system
pip install -r requirements.txt
Dependencies (requirements.txt):

nginx
Copy code
pandas
scikit-learn
numpy
▶️ Usage

Place the dataset files (movies.csv, ratings.csv, tags.csv) in your working directory.

Open and run the notebook Tak3.ipynb in Google Colab or Jupyter Notebook.

Try out the recommender:

python
Copy code
# Content-based example
print(recommend_content("Inception"))

# Collaborative example
print(recommend_collaborative(1))   # recommendations for user with ID = 1
📊 Example Output
pgsql
Copy code
🎬 Content-based (similar to 'Inception'):
['The Matrix', 'Interstellar', 'Memento', 'The Dark Knight', 'Shutter Island']

👤 Collaborative (recommendations for user 1):
['Avatar', 'The Lord of the Rings', 'The Godfather', 'Toy Story', 'The Shawshank Redemption']
📌 Future Improvements
Add Matrix Factorization (SVD, NMF) for collaborative filtering

Use Deep Learning (Autoencoders, Neural CF)

Deploy as a web app with Streamlit or Flask

Personalize hybrid recommendations with weighting

👨‍💻 Author
Israr Hussain
