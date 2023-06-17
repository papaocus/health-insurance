# health-insurance

Importing Libraries: The code begins by importing the necessary libraries such as pandas, numpy, matplotlib, seaborn, and warnings. These libraries are commonly used for data analysis and visualization tasks.

Reading the Dataset: The code reads the insurance dataset from a CSV file using the pd.read_csv() function and assigns it to the variable df. The dataset contains information about individuals' age, sex, BMI, number of children, smoking status, region, and insurance charges.

Exploring the Dataset: The code includes several commands to explore the dataset:

df.head(): Displays the first few rows of the dataset.
df.shape: Prints the dimensions of the dataset (number of rows, number of columns).
df.describe(): Provides descriptive statistics of the dataset, including count, mean, standard deviation, minimum, maximum, and quartiles.
df.dtypes: Displays the data types of each column in the dataset.
df.isnull().sum(): Counts the number of missing values in each column.
Data Visualization: The code includes multiple visualization commands using the seaborn and matplotlib libraries to create various plots:

Distribution Plot: Shows the distribution of insurance charges using histograms and kernel density estimation.
Bar Plots: Visualize the relationship between different variables (region, sex, smoker, children) and insurance charges using bar plots.
Linear Regression Plots: Shows the linear relationship between age, BMI, children, and insurance charges with separate plots for smokers and non-smokers.
Violin Plot: Displays the relationship between the number of children and insurance charges by smoker status using a violin plot.
Heatmap: Creates a correlation matrix heatmap to visualize the correlation between different variables in the dataset.
Data Preprocessing: The code performs some preprocessing steps before building a regression model:

Label Encoding: Converts categorical variables (sex, smoker, region) into numerical representations using label encoding.
Data Type Conversion: Converts the encoded variables to the appropriate data type.
Model Training and Evaluation: The code trains and evaluates regression models using the LinearRegression, Ridge, Lasso, and RandomForestRegressor algorithms. It splits the dataset into training and testing sets using train-test split and calculates the model's performance metrics, such as coefficients, intercept, and score (R-squared).

Polynomial Regression: The code applies polynomial regression by transforming the features using PolynomialFeatures. It fits a linear regression model on the transformed features and evaluates its performance using mean squared error and root mean squared error.

Final Results: The code prints the mean absolute error, mean squared error, and root mean squared error of the polynomial regression model. It also creates a DataFrame that compares the actual insurance charges with the predicted charges for the test set.
