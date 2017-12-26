# Boltzmann-Machine-Recommendation-System-for-Movies
Restricted Boltzmann Machine for collecting data and predicting whether or not a user will like a movie.
This model uses 1,000,000 ratings of movies, users and their ratings of any such movie. I've used the PyTorch library instead of tensorflow. The Boltzmann machine is trained in such a manner that whenever a new input is provided, it will tell the likelihood of a user liking that movie or not.

The Train-test Split is at 80-20 %. 

The Likelihood has been converted to boolean values. If the user gives a rating of 1 or 2, the boolean value is set to 0, indicating that the user did NOT like the movie. If the rating is 3 or greater, the boolean value is set to 1, indicating that the user likes the movie.

The parameters for optimum results are as follows (Avoids Overfitting): 

1. Number of hidden features (nh): 300
2. Batch Size : 25
3. Number of epochs : 100
4. Learning rate : Default torch learning rate
5. Evaluation : Simple Distance

The training loss : 

epoch : 1 loss: 0.015701305498646904
epoch : 2 loss: 7.655488554069901e-05
epoch : 3 loss: 5.557147661737982e-05
epoch : 4 loss: 8.071816906903986e-05
epoch : 5 loss: 2.5740203083646533e-05
epoch : 6 loss: 2.0151133009906428e-05
epoch : 7 loss: 0.0
epoch : 8 loss: 8.849714154232818e-06
epoch : 9 loss: 0.0
epoch : 10 loss: 1.9954442683459736e-05
epoch : 11 loss: 0.0
epoch : 12 loss: 0.0
epoch : 13 loss: 1.0315659170621002e-05
epoch : 14 loss: 0.0
epoch : 15 loss: 0.0
.
.
.
epoch : 90 loss: 9.433517286920429e-06
epoch : 91 loss: 0.0
epoch : 92 loss: 0.0
epoch : 93 loss: 0.0
epoch : 94 loss: 0.0
epoch : 95 loss: 0.0
epoch : 96 loss: 0.0
epoch : 97 loss: 0.0
epoch : 98 loss: 0.0
epoch : 99 loss: 0.0
epoch : 100 loss: 0.0

The test loss is 0.0



