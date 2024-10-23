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

## II. Dataset 

### 1. Context
- Fashion-MNIST is a dataset of Zalando's article images—consisting of a training set of 60,000 examples and a test set of 10,000 examples. Each example is a 28x28 grayscale image, associated with a label from 10 classes. Zalando intends Fashion-MNIST to serve as a direct drop-in replacement for the original MNIST dataset for benchmarking machine learning algorithms. It shares the same image size and structure of training and testing splits.
- The original MNIST dataset contains a lot of handwritten digits. Members of the AI/ML/Data Science community love this dataset and use it as a benchmark to validate their algorithms. In fact, MNIST is often the first dataset researchers try. "If it doesn't work on MNIST, it won't work at all", they said. "Well, if it does work on MNIST, it may still fail on others."
- Zalando seeks to replace the original MNIST dataset

### 2. Content
- Each image is 28 pixels in height and 28 pixels in width, for a total of 784 pixels in total. Each pixel has a single pixel-value associated with it, indicating the lightness or darkness of that pixel, with higher numbers meaning darker. This pixel-value is an integer between 0 and 255. The training and test data sets have 785 columns. The first column consists of the class labels (see above), and represents the article of clothing. The rest of the columns contain the pixel-values of the associated image.
-- To locate a pixel on the image, suppose that we have decomposed x as x = i * 28 + j, where i and j are integers between 0 and 27. The pixel is located on row i and column j of a 28 x 28 matrix.
-- For example, pixel31 indicates the pixel that is in the fourth column from the left, and the second row from the top, as in the ascii-diagram below.


### 3. Labels
- Each training and test example is assigned to one of the following labels:
  - 0 T-shirt/top
  - 1 Trouser
  - 2 Pullover
  - 3 Dress
  - 4 Coat
  - 5 Sandal
  - 6 Shirt
  - 7 Sneaker
  - 8 Bag
  - 9 Ankle boot
    
- TL;DR
  - Each row is a separate image
  - Column 1 is the class label.
  - Remaining columns are pixel numbers (784 total).
  - Each value is the darkness of the pixel (1 to 255)
 
    
