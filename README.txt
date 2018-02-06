
Netflix prize Collaborative Filtering System
By Stefan Himmel

- collaborative filtering machine learning algorithm to recommend movies for users based on all previous ratings by all users on all movies (from Netflix contest https://www.netflixprize.com/ )

- reccomender_system.py:
1. cleans data, splices out users that rated too few movies and movies that were rated too little
2. creates matrix of Movies by Customers, with ratings as values
3. creates x and theta feature matrices
4. specifies cost function
5. minimizes cost function using our gradient descent OR optimized fmincg function from scipy package
6. recommend top 10 movies for the specified user using the model’s highest predicted ratings

- ran data on big220 (all ratings for first 220 movies) using GPU, minimized cost as seen in cost.png