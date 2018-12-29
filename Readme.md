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