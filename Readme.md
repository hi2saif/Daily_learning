Day 0 22nd December 
Started ColumbiaX: DS102X Machine Learning for Data Science and Analytics

Day 1 23rd December
Continue Course Intro to randomiztaion

Day 2 24th December

Day 3 25th December
Update my linkedin account
Continue Course Scheduling Algorithms
Learning Python

Day 4 26th December
Continue Course Stable Marriage example
Dijktras algorithm shortest path modify
Balanced Binary Search Tree---used to find median we need to record #of nodes in the subtree for every node

Day 5 27th December
Continue to the course
Linear Programming intro objective function(maximise)
Simplex method go thorough the surface of the polyhedron till we find a point which gives optimum
Interior point method cut through middle
least square error - vertical distace from the pint to the line and squarring all
LP for Assignment probelm
NP Complete - Exponential , Approximation and Heurisitc
Personal Genomics

Day 6 28th Decemeber
Intro to machine learning 
 * classification
k-means clustering
ml is computer algorithm that searches for patterns in data
Supervised learning method --- 1) Raw Data 2) Feature Extraction 3) Mark patterns(we give examples of pattern from which the computer learns) --> 
-->Training Data or Test data -->after Training (calibratice) trained model can be applied to test data set
If line divides the two group of points and we need to see if the new point is on which side of the plane then we need to calculate the projection on the nrmal vector and see the result sign 
negative or positive
Learning means calibration -->supervised : Marked patterns are available
			   -->Unsupervised : No marked patterns
learning from more n more examples is regression problem

Classification--- classifier 
quantifying mistakes
-loss function for K classes:
 	loss: {1.....K} * {1....K} -> [0,infinity}
-Usage:loss ( f(x) ,true class of x)
- If all mistakes are equally bad:
	loss(i,j) = 1 if i=!j 0 if i=j

-If class distributions known:
	-Risk of classifier is the expected loss,
		risk(f) = E|loss(f(X) , true class of X)|

classifier type -->Nearest neighbour classification

Idea : Use Tranining data as classifier
	
	-Given: Data point x
	-Find training data point closest to x
	- Assign x the label of closest point

k-nearest neighbour (kNN)

	- Find k closest training points
	- Take a majority vote between these points
PS
: 3NN often works well

Linear Classifier: To draw the line in the middle of the two data sets we need to draw convex hall set
then the line which crosses atleast one point in the dataset and does not intersect the convex hall set is the line of middle
classifeir example support vector machine
convex hall optimisatiob problm
Support Vector machine example:(uses kernel trick to bend the line)
	Example Pincode recognisation digit recognised and automatically say what pincode it is
find the shrtest distance between the points and draw the line in the middle

Ensemble Classifier : Random Forest
for random forest we need weak classifier that is tree clasifier


Day 7 29th December: Continue the course

Model Selection: 
	Training error = number of misclassified training points / number of training points

Overfitting
classifier parameter : Tree Classifier : Number of splits
			Tree Ensemble   : Tree Parameters
					: Number of trees
			Random Forest   : Tree Parameters
					:  Number of Trees
					:  Number of random dimension
			SVM		: Hyperplane position

Example Tree:   Model : All Trees with k splits
		Parameter : Split location
		Hyperparameter : k
	the Process of choosing a hyperparameter is called a model selection 

Solution to model selection problem is cross validation
Model Selection chooses a mdel complexity( a hyperparameter)
Training a classifiesr choses parameter values

How do we select an adeuate model based on sample data?
Ans: First we would select a model if we knew the underlying distribution
then apply same principle then Approximate the sample data (this is know as cross validatin)

Data splitting estimates the prediction error from data
Model selection : optimize performance
CLassifier assessment : Interpret performance

Cross validation Steps:
Split data into three sets: Training set test set validation set
Train classifier with different hyperparameters on training set
Select the one with smallest prediction error on test set
Estimate performance on validation set

Implementation:How to split the data?
If samples assumed i.i.d split at random

Larger training set  --> More accurate classifier
Small Training set  -> Reflects variation between sample sets

K-fold cross validation

New Topic:

Probablistic Models for massive data:Efficient framework for discovering useful patterns in massive data
Probablistic Models pipline: Knowledge ->Make Assumptions -->Disccover Paaterns -> Predict and Explore
LDA is  a Probablity model of text

Stochastic variational inference methd: Massive data set -->  Subsample data  --> infer local structure  --> update global structure

-----------------------Course ended-----------------

Day 8 30th December : Siraj Raval Learn Python fo Data Science
Day 9 31st December : FA18: Computing for Data Analysis course on edX


