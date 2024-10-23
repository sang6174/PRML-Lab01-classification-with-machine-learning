# PRML-Lab01: Classification with machine learning

## I. Requirements

### 1. Data Loading & Preprocessing:
- Download the Fashion-MNIST dataset from this GitHub repo https://github.com/zalandoresearch/fashion-mnist
Perform data splitting appropriately.
- Perform techniques on transformation such as normalization, scale, drop, rotation, etc if possible and necessary.
Perform basic exploratory data analysis (EDA) to understand the distribution of classes and visualize some sample images.

### 2. Linear Model - Logistic Regression:
- Train a logistic regression classifier using all 784 features of Fashion-MNIST.
- Evaluate the model's performance on the test set, reporting key metrics like accuracy, precision, recall, F1 score, and the confusion matrix.
- Discuss any observed patterns in model performance (e.g., which items are more  easily confused).

### 3. Support Vector Machine (SVM):
- Train an SVM with a linear kernel on the same dataset and evaluate its performance.
- Train another SVM using an RBF kernel and compare the results with the linear kernel SVM and logistic regression.
- Analyze and compare computation time for training and evaluation, especially between the linear and RBF kernels.

### 4. Curse of Dimensionality & Dimensionality Reduction:
- Discuss the concept of the curse of dimensionality and its impact on machine learning models, particularly in high-dimensional feature spaces.
- Apply Principal Component Analysis (PCA) or Linear Discriminant Analysis (LDA) to reduce the dimensionality of the dataset from 784 features to a lower number (e.g., 100 or 50).
- Retrain both the logistic regression and SVM models on the reduced-dimensional data and compare their performance with the models trained on the full-dimensional data.
- Reflect on the trade-offs between dimensionality reduction and model performance.

### 5. Model Evaluation & Comparison:
- Compare the logistic regression and SVM models (linear vs. RBF kernel) on both full and reduced-dimensional data.
- Create plots to visualize model accuracy, confusion matrices, or performance metrics (precision, recall, F1 score) across different models and settings.
- Discuss the pros and cons of each model, considering aspects like accuracy, computation time, and their behavior when handling high-dimensional data.
