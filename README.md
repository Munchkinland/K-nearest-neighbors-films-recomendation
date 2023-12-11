# K-Nearest Neighbors Movie Recommendation System

![Alt text](image.png)

This repository contains a movie recommendation system based on the K-Nearest Neighbors (KNN) algorithm implemented in Python. The system uses movie data from the TMDb (The Movie Database) for recommending similar movies based on user preferences.

🙋‍♂️Steps to Run the System
Follow these steps to run the movie recommendation system:

1. Data Ingestion

In the first step, movie and credit data is downloaded from the TMDb database. The data is stored in CSV files for further processing.

2. Database Creation

In this step, an SQLite database is created, and movie and credit data are loaded into separate tables. Then, a join operation is performed on the tables to create a combined DataFrame containing movie information such as title, description, genres, keywords, cast, and crew.

3. Data Transformation

Various data transformations are applied to prepare the data for modeling. This includes extracting names from JSON lists, text cleaning, and creating a "tags" column that combines multiple relevant features.

4. KNN Model Creation

In this step, a KNN model is created using the scikit-learn library. The model uses the TF-IDF matrix of movie tags to find similar movies based on cosine similarity.

5. Movie List Query

Finally, the user can input a movie title, and the system will provide a list of movie recommendations based on the KNN model.

🧐Repository Structure
- data/raw: Contains the original CSV files with movie and credit data.
- models: Contains the trained KNN model (knn_model.pkl).
- src: Contains the source code for the recommendation system.
- utils.py: Utility functions for database connection and other operations.
- explore.ipynb: The original Jupyter notebook containing the code before being converted to a Python script.
- main.py: The main script that runs the recommendation system.

🖥Running the System

To run the movie recommendation system, follow these steps:

✅Clone this repository to your local machine.
✅Ensure you have Python installed on your system.
✅Install the required libraries by running pip install -r requirements.txt.
✅Run the system by executing python src/main.py.

📊Additional Notes

The recommendation system is based on the KNN algorithm and uses the TF-IDF matrix to calculate similarity between movies.

Movie data is obtained from the TMDb database and is used for educational and demonstration purposes.

You can customize and fine-tune the system for your own data or needs.

Enjoy exploring and using this KNN-based movie recommendation system!