# Neural_Network_Charity_Analysis

# Overview of Project

Beks has come a long way since her first day at that boot camp five years ago—and since earlier this week, when she started learning about neural networks! Now, she is finally ready to put her skills to work to help the foundation predict where to make investments.

With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

* EIN and NAME—Identification columns
* APPLICATION_TYPE—Alphabet Soup application type
* AFFILIATION—Affiliated sector of industry
* CLASSIFICATION—Government organization classification
* USE_CASE—Use case for funding
* ORGANIZATION—Organization type
* STATUS—Active status
* INCOME_AMT—Income classification
* SPECIAL_CONSIDERATIONS—Special consideration for application
* ASK_AMT—Funding amount requested
* IS_SUCCESSFUL—Was the money used effectively


# Deliverables 

* Deliverable 1: Preprocessing Data for a Neural Network Model
* Deliverable 2: Compile, Train, and Evaluate the Model
* Deliverable 3: Optimize the Model
* Deliverable 4: A Written Report on the Neural Network Model (README.md)

# Resources

* Data Source: charity_data.csv, AlphabetSoupCharity.h5 and AlphabetSoupCharity_Optimzation.h5
* Data Tools: AlphabetSoupCharity_starter_code.ipynb, AlphabetSoupCharity.ipynb and AlphabetSoupCharity_Optimzation.ipynb.
* Software: Python 3.9, Visual Studio Code 1.50.0, Anaconda 4.8.5, Jupyter Notebook 6.1.4 and Pandas

# Deliverable 1

1.) Read in the charity_data.csv to a Pandas DataFrame, and be sure to identify the following in your dataset:
  * What variable(s) are considered the target(s) for your model?
  * What variable(s) are considered the feature(s) for your model?
2.) Drop the EIN and NAME columns.
3.) Determine the number of unique values for each column.
4.) For those columns that have more than 10 unique values, determine the number of data points for each unique value.
5.) Create a density plot to determine the distribution of the column values.
6.) Use the density plot to create a cutoff point to bin "rare" categorical variables together in a new column, Other, and then check if the binning was successful.
7.) Generate a list of categorical variables.
8.) Encode categorical variables using one-hot encoding, and place the variables in a new DataFrame.
9.) Merge the one-hot encoding DataFrame with the original DataFrame, and drop the originals.
