# Dimension Reduction

Before going into details and codes, the very first question asking by the management or non Data Science guy is - 
What is Dimension Reduction and why this is so important?
Before modeling any algorithm, the very basic step is to preprocess the dataset. People call it with different names like Exploritory Data Analysis(EDA), Data Prepration, Data Analysis etc. Suppose while doing the EDA, we get to know that there are 50 features in the dataset. Next question will be, should we take the all features or just drop few randomly and proceed further. While doing the EDA, ever the domain expert with 30 years of experience can't say take these five out of fifty feature and make a model. And if we will take all features, it will be computationally very expensive and there might be a chance of poor performance. To address this problem, Dimension Reduction came to the picture.
Dimension reduction will reduce the feature by taking few features (called principal components) which are most relevant for the algorithm.

# Methods of Dimensionality Reduction
There are various methods for Dimension Reduction, here i will be discussing about three popular ways of Dimension Reduction namely - 
Principal Component Analysis (PCA)
Linear Discriminant Analysis (LDA) 
t-distributed Stochastic Neighbour Embedding (t-SNE)

# Principal Component Analysis (PCA)
•	As per wikipedia, it is a statistical procedure that utilise orthogonal transformation to convert a set of observations of possibly correlated variables (entities each of which takes on various numerical values) into a set of values of linearly uncorrelated variables called principal components. 
• In simple words, convert possible correlated features (predictors) into linearly uncorrelated features (predictors) called principal components
• Linear dimensionality reduction using Singular Value Decomposition of the data to project it to a lower dimensional space
• Number of principal components <= number of features (predictors)
• First principal component explains the largest possible variance
•	Each subsequent component has the highest variance subject to the restriction that it must be orthogonal to the preceding components
• Used in exploratory data analysis (EDA)
• Used in Feature extraction and engineering
• Used in Noise filtering
• Used in Visualization

# Linear Discriminant Analysis (LDA)
• As per wikipedia, it is a method used in statistics, pattern recognition and machine learning to find a linear combination of features that characterizes or separates two or more classes of objects or events. The resulting combination may be used as a linear classifier, or, more commonly, for dimensionality reduction before later classification.
• Also known as Linear discriminant analysis (LDA), normal discriminant analysis (NDA), or discriminant function analysis (DFA)
•	Most commonly used as dimensionality reduction technique in the pre-processing step for pattern-classification and machine learning applications. 
•	Goal is to project a dataset onto a lower-dimensional space with good class-separability in order avoid overfitting (“curse of dimensionality”) and also reduce computational costs.
•	Locate the 'boundaries' around clusters of classes. 
•	Projects data points on a line
•	A centroid will be allocated to each cluster or have a centroid nearby

# t-distributed Stochastic Neighbor Embedding (t-SNE)
•	Nonlinear dimensionality reduction technique that is particularly well-suited for embedding high-dimensional data into a space of two or three dimensions, which can then be visualized in a scatter plot. 
•	Models each high-dimensional object by a two- or three-dimensional point in such a way that similar objects are modeled by nearby points and dissimilar objects are modeled by distant points. dimensional space (e.g., to visualize the MNIST images in 2D).
