# movie-Recommendation-System-with-Netflix-

Problem Statement
Netflix provided a lot of anonymous rating data, and a prediction accuracy bar that is 10% better than what Cinematch can do on the same training data set. (Accuracy is a measurement of how closely predicted ratings of movies match subsequent actual ratings.)

Problem Description
Netflix is all about connecting people to the movies they love. To help customers find those movies, they developed 
world-class movie recommendation system: CinematchSM. Its job is to predict whether someone will enjoy a movie 
based on how much they liked or disliked other movies. Netflix use those predictions to make personal movie recommendations based on each customer’s unique tastes.
And while Cinematch is doing pretty well, it can always be made better.

Now there are a lot of interesting alternative approaches to how Cinematch works that netflix haven’t tried. Some are described in the literature,
some aren’t. We’re curious whether any of these can beat Cinematch by making better predictions. 
Because, frankly, if there is a much better approach it could make a big difference to our customers and our business.

Exploratory Data Analysis
Preprocessing
Spliting data into Train and Test(80:20)
Exploratory Data Analysis on Train data
Distribution of ratings
Number of Ratings per a month
Analysis on the Ratings given by user
Analysis of ratings of a movie given by a user
number of ratings on each day of the week
Creating sparse matrix from data frame
Finding Global average of all movie ratings, Average rating per user, and Average rating per movie
Cold Start problem
Computing Similarity matrices
Computing User-User Similarity matrix
Calculating User User Similarity_Matrix is not very easy(unless you have huge Computing Power and lots of time) because of number of. usersbeing lare.
    You can try if you want to. Your system could crash or the program stops with Memory Error
Trying with all dimensions (17k dimensions per user)
Trying with reduced dimensions (Using TruncatedSVD for dimensionality reduction of user vector)
Computing Movie-Movie Similarity matrix
Even though we have similarity measure of each movie, with all other movies, We generally don't care much about least similar movies.

Most of the times, only top_xxx similar items matters. It may be 10 or 100.

We take only those top similar movie ratings and store them in a saperate dictionary.
Finding most similar movies using similarity matrix
Does Similarity really works as the way we expected...? Let's pick some random movie and check for its similar movies.

Machine Learning Models
Sampling Data
Build sample train data from the train data
Build sample test data from the test data4.2 Finding Global Average of all movie ratings, Average rating per User, and Average rating per Movie (from sampled train)
Finding Global Average of all movie ratings, Average rating per User, and Average rating per Movie (from sampled train)
