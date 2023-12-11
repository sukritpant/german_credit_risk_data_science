# German Credit Risk Project #


The project analyzes the German Credit Risk data available in Kaggle through use of various graphical visualization and statistical test. This project was performed as a part of Integrify Data Science and Machine Learning Project when I was part of the program. The purpose of this is to analyze various information regarding why German people take 'consumer loans'.

## About the Dateset ##

The dataset was taken from Kaggle <https://www.kaggle.com/datasets/uciml/german-credit> as a CSV file and loaded into a Jupyter Notebook. The following columns are available in the dataset:
1. Age (Numerical: Integer): between 18-75
2. Sex (Categorical): Male and Female
3. Job (Categorical): Number 0 through 3 with following labels: 0>> unskilled and non-resident, 1>>unskilled resident, 2>>skilled, 3>>highly skilled
4. Housing (Categorical): Own, Rent, Free
5. Saving Accounts (Categorical): NaN,little, moderate, quite rich, rich
6. Checking account (Categorical): NaN,little, moderate, quite rich, rich
7. Credit amount (Numerical: Float): Duestche Mark
8. Duration (Numerical: Integer): in months
9. Purpose (Categorical): car, furniture/equipment, radio/TV, domestic appliances, repairs, education, business, vacations/others

### Packages
Packages loaded for these analysis are as follows but not all the packages have been utilized:
- pandas
- numpy
- seaborn
- matplotlib
- datetime
- time
- scipy
- sklearn

## Data Exploration
There are some missing values in the Saving Accounts and Checking Accounts which were filled by No Account Available as a lot of information would be lost if these rows were dropped but it would still be interesting to see if No Account Available would also have some kind of impact on the consumer loan.

### Data Visualization
All the various columns have been charted to extract relevant information along with a correlation matrix for numerical variables to see if there is something interesting that can be extracted from the information. Similarly further analysis was made regarding the outliers in the various numerical data.

### Hypothesis Testing
After exploring and visualizing the data, there was a need to perform hypothesis testing to see if there is a significant different between the credit amount for various purpose of loan. The data was checked for normality through Shapiro test which the dataset failed. Though the data was not normally distributed, an assumption on normality was made before performing a one-way ANOVA Test. After the proof of significance, a further data visualization is performed to analyze the differences between credit amount and purpose of loan.

## Reflection
As this was an initial data analysis and exploration done on a new dataset, the visualization was performed  to check for the various information that are available in the data. Even without the goal in view, there is a possibility to explore and visualize the various data and also a hypothesis can be crafted and tested in similar data.
