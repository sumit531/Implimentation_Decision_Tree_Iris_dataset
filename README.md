# Implimentation_Decision_Tree_Iris_dataset
Certainly, here's a step-by-step summary of the decision tree model creation process in the provided code:

1. **Loading the Iris Dataset:**
   - The `load_iris` function from `sklearn.datasets` is used to load the Iris dataset.
   - The features (X) are assigned to `iris.data`.
   - The target labels (y) are assigned to `iris.target`.

2. **Splitting the Dataset:**
   - The `train_test_split` function from `sklearn.model_selection` is used to split the dataset into training and testing sets.
   - The features and labels are split into `X_train`, `X_test`, `y_train`, and `y_test`, with a test size of 20%.

3. **Checking Data Shapes:**
   - The `.shape` attribute is used to print the shapes of the training and testing data arrays as well as the training labels.

4. **Creating a Decision Tree Classifier:**
   - An instance of `DecisionTreeClassifier` from `sklearn.tree` is created and assigned to `clf`.

5. **Training the Decision Tree:**
   - The `fit` method of the classifier is called with the training data and labels (`X_train` and `y_train`) to train the decision tree model.

6. **Making Predictions:**
   - The `predict` method of the trained classifier is used to make predictions on the testing data (`X_test`), and the predictions are stored in `y_pred`.

7. **Calculating Accuracy:**
   - The `accuracy_score` function from `sklearn.metrics` is used to calculate the accuracy of the model's predictions (`y_pred`) compared to the actual testing labels (`y_test`).

8. **Visualizing the Decision Tree:**
   - The `plot_tree` function from `sklearn.tree` is used to visualize the trained decision tree classifier.
   - The size of the plot is adjusted using `rcParams` from `matplotlib.pyplot`.

The output of the `plot_tree` function provides a visual representation of the decision tree's structure. Each node in the tree corresponds to a decision rule based on a specific feature and threshold. The tree is split based on these rules until leaf nodes are reached, which represent the predicted class labels. The Gini impurity measure is used to determine the best splits at each node.

Lastly, the accuracy of the model is calculated and reported as 0.96, indicating that the model's predictions matched the actual testing labels with an accuracy of 96%.
