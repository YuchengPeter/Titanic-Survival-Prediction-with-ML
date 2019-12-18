# Titanic-Survival-Prediction-with-ML
Using machine learning to predict whether a passenger will survive the titanic event

Data source: Kaggle https://www.kaggle.com/c/titanic

1. A single DT is trained and has around 80% accuracy on testing data. Challenges I have encountered: 
	- Missing data: Currently, I am filling all missing data with 0. It is not the ideal approach, however, because it affects the split of      feature with missing data. Will re-approach this issue later.
	- I am manually dropping features that I believe holds no value(the name of the passenger, passenger ID, ticket number, etc.). However,      this will not be feasible when the number of features grow significantly. Plus, my intuition could be wrong. Perhaps PCA would be a        solution to eliminate useless features. 
	- In the future, I will visualize my decision tree to see if there's any contraints I could add to my DT(max depth, min number of leaf        nodes, entropy vs gini, etc.)

2. I have implemented a random forest model with minimum modification from sklearn's default parameters. The next step would be to learn how to modify the parameters to improve the performance of the model.  

3. Once I am done with decision tree implementation, I will use neural network and see how the two machine learning techniques perform differently. 
