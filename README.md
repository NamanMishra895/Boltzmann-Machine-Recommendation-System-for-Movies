# Boltzmann-Machine-Recommendation-System-for-Movies
Restricted Boltzmann Machine for collecting data and predicting whether or not a user will like a movie.
This model uses 1,000,000 ratings of movies, users and their ratings of any such movie. I've used the PyTorch library instead of tensorflow. The Boltzmann machine is trained in such a manner that whenever a new input is provided, it will tell the likelihood of a user liking that movie or not.

The Train-test Split is at 80-20 %. u1.base (80k ratings) is the training data and u1.test (20k ratings) is the test data.

The Likelihood has been converted to boolean values. If the user gives a rating of 1 or 2, the boolean value is set to 0, indicating that the user did NOT like the movie. If the rating is 3 or greater, the boolean value is set to 1, indicating that the user likes the movie.

