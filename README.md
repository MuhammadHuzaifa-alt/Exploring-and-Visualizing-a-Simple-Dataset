# Exploring-and-Visualizing-a-Simple-Dataset
Learn how to load, inspect and visualize a dataset to understand data trends and distributions
Iris Dataset Exploratory Data Analysis (EDA)

This project performs Exploratory Data Analysis (EDA) on the famous Iris dataset using Pandas, Seaborn, and Matplotlib in Python.

The analysis includes:

Dataset inspection
Statistical summary
Pairplot visualization
Histograms
Boxplots
Technologies Used
Python
Pandas
Seaborn
Matplotlib
Dataset

The project uses the built-in Iris dataset available in Seaborn.

Dataset contains:

Sepal Length
Sepal Width
Petal Length
Petal Width
Species

Species included:
Setosa
Versicolor
Virginica
Features of the Project
Load and explore dataset
Display dataset shape and columns
View first few rows
Check dataset information
Generate statistical summary
Create pairplot for species comparison
Visualize feature distributions using histograms
Detect outliers using boxplots
Project Structure
iris-eda/
│
├── iris_analysis.py
├── README.md
Installation
Clone Repository
git clone https://github.com/your-username/iris-eda.git
cd iris-eda
Install Required Libraries
pip install pandas seaborn matplotlib
Run the Project
python iris_analysis.py
Code Explanation
1.Load Dataset
df = sns.load_dataset("iris")

Loads the Iris dataset from Seaborn.
2.Dataset Information
print(df.shape)
print(df.columns)
df.head()

Displays:
Number of rows and columns
Dataset column names
First 5 records
3. Dataset Statistics
print(df.info())
print(df.describe())

Shows:

Data types
Null values
Statistical summary
4.Pairplot Visualization
sns.pairplot(df, hue='species')

Creates scatter plots for feature relationships and color-codes species.
5.Histograms
sns.histplot(df[i], bins=15)
Displays feature distributions using histograms.
6.Boxplots
sns.boxplot(df[features[x]])
Shows data spread and detects outliers.
Output Visualizations
The project generates:
Pairplots
Histograms
Boxplots
These visualizations help understand:
Data distribution
Feature relationships
Outliers
Species separation
Example Output
Dataset Shape
(150, 5)
Future Improvements
Add machine learning models
Perform feature engineering
Add correlation heatmap
Create interactive dashboard
Export visualizations
Author
Muhammad Huzaifa

Python Developer
Data Science Enthusiast
Machine Learning Learner
