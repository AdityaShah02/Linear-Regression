# Linear Regression 

This repository contains implementations of both Simple and Multiple Linear Regression in Python using sample datasets. The goal is to showcase the process of linear regression for predictive modeling.

## Simple Linear Regression

### File
1. **LinearRegression_Simple.ipynb**
   - Jupyter Notebook containing the implementation of Simple Linear Regression.
   - Demonstrates the process from loading the dataset to plotting the best-fit line.
  
### Dataset
The Simple Linear Regression project uses a salary dataset (`Salary_dataset.csv`) with columns for `YearsExperience` and `Salary`. The dataset is located in the `data` directory.

### Getting Started
To run the notebook locally, you can use Google Colab or any Jupyter Notebook environment. If using Colab, make sure to mount your Google Drive as shown in the notebook.

```python
from google.colab import drive
drive.mount('/content/drive')
```
Ensure you have the necessary dependencies installed:

```bash
pip install numpy pandas matplotlib
```

#### Code Explanation

1. **Loading and Visualizing the Data**
   - The dataset is loaded using Pandas from the provided CSV file. (add the path of the dataset provided)
   - The relationship between years of experience and salary is visualized using Matplotlib.

2. **Adding Intercept Term**
   - To perform linear regression in vectorized form, an intercept term is added to the feature matrix. This is necessary for the model to learn both the slope and the intercept during training.

3. **Cost Function**
   - The cost function is defined to evaluate the performance of the model. It calculates the mean squared error between the predicted and actual values.
  
4. **Gradient Descent**
   - Gradient descent is implemented to optimize the model parameters (slope and intercept). It iteratively updates the parameters to minimize the cost function.

5. **Results**
   - The final model parameters (M and C) are printed.
   - The best-fit line is plotted along with the original data points.

#### Running the Code

Open the Jupyter Notebook (LinearRegression_Simple.ipynb) and execute the cells sequentially. This will walk you through each step of the Simple Linear Regression process.

#### Results

The final model parameters (M and C) are printed, and the best-fit line is plotted along with the original data points.


## Multiple Linear Regression
### File

2. **LinearRegression_Multiple.ipynb**
   - Jupyter Notebook containing the implementation of Multiple Linear Regression.
   - Utilizes two features (fixed acidity and volatile acidity) to predict the quality of wine.

### Dataset

The Multiple Linear Regression project uses a wine quality dataset (winequality-red.csv) with various features related to wine characteristics. The dataset is located in the data directory.
Getting Started

Similar to the Simple Linear Regression project, run the necessary commands to mount Google Drive and install dependencies if required.

```python
from google.colab import drive
drive.mount('/content/drive')
```

### Code Explanation

1. **Loading and Visualizing the Data**
   - The dataset is loaded using Pandas from the provided CSV file.
   - Features (fixed acidity and volatile acidity) and the target variable (quality) are selected.
2. **Converting Table to Arrays**
   - The feature matrix (X) is created by adding an intercept term and converting it to a NumPy array.
3. **Gradient Descent**
   - Gradient descent is implemented to optimize the model parameters (theta). It iteratively updates the parameters to minimize the cost function.
4. **3D Plotting**
   - A 3D plot is created to visualize the relationship between two features (fixed acidity and volatile acidity) and the target variable (quality).

5. **Results**
   - The final model parameters (theta0, theta1, and theta2) are printed.
   - The cost function is visualized over iterations, and the best-fit plane is plotted in a 3D graph.

#### Running the Code
Open the Jupyter Notebook (LinearRegression_Multiple.ipynb) and execute the cells sequentially. This will guide you through the process of Multiple Linear Regression.
Results

The final model parameters (theta0, theta1, and theta2) are printed, and the cost function is visualized over iterations. The best-fit plane is plotted in a 3D graph.
Contributing

**Everything added in this repository is correct to my best knowledge. Still if you come across any error(s), feel free to suggest the corrections on the mail address shah.adity072@gmail.com .**
