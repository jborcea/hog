# projects
# The Game of Hog
In Hog, two players alternate turns trying to be the first to end a turn with at least GOAL total points, 
where GOAL defaults to 100. On each turn, the current player chooses some number of dice to roll, up to 10. 
That player's score for the turn is the sum of the dice outcomes. However, a player who rolls too many dice risks:

1. Sow Sad. If any of the dice outcomes is a 1, the current player's score for the turn is 1.

In a normal game of Hog, those are all the rules. To spice up the game, we'll include some special rules:

2. Pig Tail. A player who chooses to roll zero dice scores 2 * abs(tens - ones) + 1 points; where tens, 
ones are the tens and ones digits of the opponent's score. The ones digit refers to the rightmost digit 
and the tens digit refers to the second-rightmost digit.
3. Square Swine. After a player gains points for their turn, if the resulting score is a perfect square, 
then increase their score to the next higher perfect square. 
A perfect square is any integer n where n = d * d for some integer d.

# Yelp Maps
In this project, you will create a visualization of restaurant ratings using machine learning and the Yelp academic dataset. 
In this visualization, Berkeley is segmented into regions, where each region is shaded by the predicted rating of the closest restaurant 
(yellow is 5 stars, blue is 1 star). Specifically, the visualization you will be constructing is a Voronoi diagram.

In the map above, each dot represents a restaurant. The color of the dot is determined by the restaurant's location. 
For example, downtown restaurants are colored green. The user that generated this map has a strong preference for Southside restaurants, 
and so the southern regions are colored yellow.

This project uses concepts from Sections 2.1, 2.2, 2.3, and 2.4.3 of Composing Programs. 
It also introduces techniques and concepts from machine learning, a growing field at the intersection of 
computer science and statistics that analyzes data to find patterns and make predictions.

The maps.zip archive contains all the starter code and data sets. 
The project uses several files, but all of your changes will be made to utils.py, abstractions.py, and recommend.py.

abstractions.py: Data abstractions used in the project
recommend.py: Machine learning algorithms and data processing
utils.py: Utility functions for data processing
ucb.py: Utility functions for miscellaneous and debugging
data: A directory of Yelp users, restaurants, and reviews
ok: The autograder
proj1.ok: The ok configuration file
tests: A directory of tests used by ok
users: A directory of user files
visualize: A directory of tools for drawing the final visualization

# Movie Classification
You will build a classifier that guesses whether a movie is romance or action, using only the numbers of times words appear in the movies's screenplay. 
By the end of the project, you should know how to:

1. Build a k-nearest-neighbors classifier.
2. Test a classifier on data.
