import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

df = sns.load_dataset('iris')
print(df.shape)
print(df.columns)
print(df.head())
print(df.info())
print(df.describe())

plt.figure(figsize=(6,4))
sns.scatterplot(data=df, x='sepal_length', y='petal_length', hue='species')
plt.title('Sepal Length vs Petal Length')
plt.show()

df.hist(figsize=(8,6))
plt.suptitle('Feature Distributions', y=1.02)
plt.show()

plt.figure(figsize=(8,6))
sns.boxplot(data=df)
plt.title('Box Plot of Iris Features')
plt.show()
This task was completed by first loading the Iris dataset using pandas and exploring its basic structure through shape, column names, head(), info(), and describe() to understand the data types, sample records, and statistical summary. Then, different visualizations were created using matplotlib and seaborn to examine trends and patterns in the data. A scatter plot was used to show the relationship between sepal length and petal length based on species. Histograms were generated to display the distribution of each numeric feature, and box plots helped identify possible outliers and compare feature spread. These steps provided a clear understanding of the dataset's structure, distribution, and feature relationships.
