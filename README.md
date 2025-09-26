# The classification of iris flowers
In this section, we are going to work through a small machine learning project end-to-end.  Here is an overview of what we are going to cover:      Installing the Python and SciPy platform.     Loading the dataset.     Summarizing the dataset.     Visualizing the dataset.     Evaluating some algorithms.     Making some predictions.
# Summarize the Dataset
  shape:(150, 5)
  Peek at the Data:<img width="576" height="464" alt="Screenshot 2025-09-26 at 14 10 08" src="https://github.com/user-attachments/assets/dab9709f-4bca-4806-9c90-02a8b962bbe6" />
  
  Statistical Summary:<img width="491" height="205" alt="Screenshot 2025-09-26 at 14 10 55" src="https://github.com/user-attachments/assets/3ef1b59f-7e89-4566-ba29-d50726f41463" />
  
  Class Distribution: <img width="278" height="112" alt="Screenshot 2025-09-26 at 14 11 32" src="https://github.com/user-attachments/assets/a536a409-905a-4af4-896b-cb8c4f32d56c" />

# Data Visualization
I used Univariate plots to better understand each attribute.
-Given that the input variables are numeric, I create box and whisker plots of each

<img width="629" height="472" alt="Screenshot 2025-09-26 at 14 02 07" src="https://github.com/user-attachments/assets/7b8827f7-e2c1-4ce8-a5ee-ed78763e74e5" />

-Histogram: It looks like perhaps two of the input variables have a Gaussian distribution.

<img width="629" height="471" alt="Screenshot 2025-09-26 at 14 06 17" src="https://github.com/user-attachments/assets/015b13bc-811e-4b82-b75f-57847d832bd9" />

- Multivariate Plots: Note the diagonal grouping of some pairs of attributes. This suggests a high correlation and a predictable relationship.
-Scatter Matrix Plot for Each Input Variable for the Iris Flowers Dataset

<img width="624" height="467" alt="Screenshot 2025-09-26 at 14 07 30" src="https://github.com/user-attachments/assets/b04be6c8-d369-47a7-9de1-c4b0cf6b06f9" />

# Evaluate Some Algorithms
We need to know that the model we created is good.We will split the loaded dataset into two, 80% of which we will use to train, evaluate and select among our models, and 20% that we will hold back as a validation dataset.Then We will use stratified 10-fold cross validation to estimate model accuracy.
We get an idea from the plots that some of the classes are partially linearly separable in some dimensions, so we are expecting generally good results.

Let’s test 6 different algorithms:

    Logistic Regression (LR)
    Linear Discriminant Analysis (LDA)
    K-Nearest Neighbors (KNN).
    Classification and Regression Trees (CART).
    Gaussian Naive Bayes (NB).
    Support Vector Machines (SVM).

This is a good mixture of simple linear (LR and LDA), nonlinear (KNN, CART, NB and SVM) algorithms.

6 models and accuracy estimations for each.<img width="257" height="136" alt="Screenshot 2025-09-26 at 14 15 29" src="https://github.com/user-attachments/assets/abd05e53-0e7b-4767-9488-0856afbca0c7" />

# the classification report 
the classification report provides a breakdown of each class by precision, recall, f1-score and support showing excellent results (granted the validation dataset was small).

<img width="482" height="295" alt="Screenshot 2025-09-26 at 14 17 02" src="https://github.com/user-attachments/assets/19d05f6d-c659-4b85-b092-5cf07e0bb071" />
