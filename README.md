# Adult-Income-Dataset
# This data set is picked from below

UCI Machine Learning Repository. (n.d). Social Data Sets. Retrieved [02/05/2024], from https://archive.ics.uci.edu/dataset/2/adult

Number of Variables: 15
Size of Data Set: 48842 instances

The idea is to analyze the data with different statistical models and check that population distribution of income >50K exceeds 0.25 on number of years of education greater than its mean.

The below checks are done
1. Checking mean, standard deviation and variance of sample.
2. Various histogram plots.
3. Probability Distributions based on various explanatory variables and finding correlation.
4. Sampling Distribution and Central Limit Theorem  
5. Wald and Scope Confidence intervals
6. Significance Tests, checking P-value, Z-Test and chi-squared tests.
7. Fitting Linear Regression
8. Fitting Generalized Linear Models
9. Conclusion on result of population distribution

# Use the commands below in python to fetch data and view the metadata and data types of variables

from ucimlrepo import fetch_ucirepo
# fetch dataset
adult = fetch_ucirepo(id=2)
# data (as pandas dataframes)
X = adult.data.features
y = adult.data.targets
# metadata
print(adult.metadata)
# variable information
print(adult.variables)


