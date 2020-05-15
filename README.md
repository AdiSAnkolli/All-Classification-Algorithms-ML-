#All Classification Algorithms:-


I'm Planning to implement all these classification algorithms on a dataset which contains all stats of pokemons of first 5 generations!!
Interesting, isn't it? But what will my algorithm classify/predict? Well,my algorithms will predict whether the pokemon is legendary or not based on all the stats mentioned in the dataset!! If possible, i'll visualize all the results on Orange Data Mining/ Data Visualization tool for a better understanding, and it will also give an exciting feeling to it!!
Let's get right into it then!!!


1) Decison Tree:-
A decision tree is a flowchart-like structure in which each internal node represents a "test" on an attribute (e.g. whether a coin flip comes up heads or tails), each branch represents the outcome of the test, and each leaf node represents a class label (decision taken after computing all attributes).
So, in this scenario, the class label, or the column that is to be predicted is the "Legendary" column which states whether the pokemon is legendary or not. Do check out the Tree Viewer in the ows file, which will precisely show you the nodes,which means, in this scenario, it will show you exactly what factors makes a pokemon legendary.


2) KNN (K-Nearest Neighbour):-
K nearest neighbors is a simple algorithm that stores all available cases and classifies new cases based on a similarity measure (e.g., distance functions). KNN has been used in statistical estimation and pattern recognition already in the beginning of 1970's as a non-parametric technique.
What KNN does is, it calculates distance (it can be Euclidean, Manhattan, etc. i went ahead with Euclidean) of every attribute (i.e column) of a new entry or test data, from every other previous entry, and then lists down specified (n) number of tuples that are closest to the new or test data. Out of those n tuples, the class label (or target variable) which appears the most is given to the new/test data. It works better when feature variables (the attributes which are studied) are numeric and the target variable (the attribute which is predicted) is a categorical value. Do check out the Linear Projection in ows file,and play around with it!! You'll never know, you might find something new and interesting!!!


3) Naive Bayes (Gaussian):-
In machine learning, naïve Bayes classifiers are a family of simple "probabilistic classifiers" based on applying Bayes' theorem with strong (naive) independence assumptions between the features. It works on the conditional probability principle. The formula for conditional probability is given by Bayes Theorem:-
P(A|B) = (P(B|A)*P(A))/P(B)  
where-
A,B are events
P(A|B) is probability of A given that B is True
P(B|A) is probability of B given that A is True
P(A),P(B) are individual probabilities of A and B
How will that help us in predicting whether a pokemon is legendary or not? Now, comditional probability of whether a pokemon is legendary or not legendary will be calculated, with respect to the stats provided in the training data. If the probability of pokemon with current stats being legendary is higher than it not being legendary, then it is deemed/predicted as legendary, and vice versa.
The reason i went ahead with Gaussian Naive Bayes is that it works better for numerical values, and it is the easiest to implement.
