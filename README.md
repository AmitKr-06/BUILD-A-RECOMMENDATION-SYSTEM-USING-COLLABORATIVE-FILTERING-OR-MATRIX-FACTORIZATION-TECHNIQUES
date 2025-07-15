# BUILD-A-RECOMMENDATION-SYSTEM-USING-COLLABORATIVE-FILTERING-OR-MATRIX-FACTORIZATION-TECHNIQUES
COMPANY: CODTECH IT SOLUTIONS 
NAME: AMIT KUMAR 
INTERN ID: CTO8DH672 
DOMAIN: MACHINE LEARNING 
DURATION: 4 WEEKS 
MENTOR: NEELA SANTOSH

EXPLANATION :
In this task, the goal is to build a recommendation system using collaborative filtering - specifically, matrix factorization using SVD (Singular Value Decomposition). I have used the MovieLens 100K dataset, which contains movie ratings from 943 users for 1,682 movies. The aim is to recommend movies to users based on the preferences of similar users.
This kind of system is used by platforms like Netflix, Amazon, and Spotify to personalize recommendations.
Step 1: Import Required Libraries
I used Pandas,Numpy,andMatplotlib
Step 2: Load the Dataset
next, step is to load the built-in MovieLens 100K dataset using the surprise library.
This dataset includes user IDs, movie IDs, and the rating (1–5) that a user gave to a movie.
Step 3: Choose the Model
I use the SVD algorithm, a matrix factorization method that breaks down the user-item rating matrix into smaller matrices to uncover hidden relationships between users and items.
Step 4: Split the Data
Then, divide the dataset into training and testing parts using Surprise’s train_test_split.
Step 5: Make Predictions
After training, i ask the model to predict ratings for the test data.
Step 6: Evaluate the Model
I Measure how accurate the model is by calculating the Root Mean Squared Error (RMSE). A lower RMSE means better performance.
Step 7: Generate Recommendations
Then, I make actual recommendations. And Assume to recommend movies for user 196. 
First, I list all the movies, then predict how user 196 would rate them, and finally pick the top 5 highest-rated movies.
Step 9: Visualizing Rating Distribution using Histogram 
I use Histogram to visualized the distribution of movie ratings.
A histogram is a type of bar chart that shows how frequently data falls into certain value ranges (bins).
Each bin corresponds to a rating value (like 1, 2, 3, 4, 5).
 OUTPUT:
 
