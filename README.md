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
 Step 1: Understand the Data
I used the MovieLens 100K dataset, which contains 100,000 ratings by 943 users for 1682 different movies. 
The main file, u.data, includes information like user ID, movie ID, rating (1 to 5), and a timestamp. 
Another file, u.item, maps movie IDs to their titles (like "Toy Story (1995)").
Step 2: Read and Prepare the Data
Then used the pandas library to read the u.data file into a DataFrame. Carefully handled file paths and encoding to avoid errors. 
Then, loaded this DataFrame into the surprise library's format using the Reader class, specifying the rating scale from 1 to 5.
Step 3: Train the Model
Next, split the dataset into a training and test set using train_test_split() from surprise.model_selection. 
Then, I used the SVD model, which is a powerful technique from linear algebra that reduces high-dimensional user-item interactions into latent features.
It figures out patterns in how users rate items. trained this model using .fit() on the training data.
Step 4: Make Predictions and Evaluate
Then, I used the trained model to predict ratings on the test set and evaluated the predictions using RMSE (Root Mean Square Error). 
A lower RMSE means the model is doing a better job predicting how users would rate unseen movies.
Step 5: Recommend Movies
Once the model was trained, I picked a user (e.g., user ID 196), then predicted ratings for all movies the user has not rated yet.
And sorted the predictions to find the top 5 highest-rated movies and printed them. These are the model’s recommendations.
Step 6: Match Movie Titles
To make the output more human-friendly, we matched the movie IDs to their actual titles using the u.item file. 
And merged this data with our top 5 predictions and printed both the movie title and predicted rating.
 Step 7: Visualization
And Finally, Plotted a histogram of all ratings using matplotlib to see the distribution. 
Most users gave ratings between 3 and 5, which shows a tendency toward liking movies.

 OUTPUT:
 <img width="1825" height="845" alt="Image" src="https://github.com/user-attachments/assets/a5146e67-8c51-498a-a5ed-40185efc9a94" />
