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

# Deliverable 1: Preprocessing Data for a Neural Network Model

1.) Read in the charity_data.csv to a Pandas DataFrame, and be sure to identify the following in your dataset:
  * What variable(s) are considered the target(s) for your model?
  * What variable(s) are considered the feature(s) for your model?

![image](https://user-images.githubusercontent.com/89880015/150660232-87307f48-6f19-477a-941e-8bc0b8ec6e38.png)

2.) Drop the EIN and NAME columns.

![image](https://user-images.githubusercontent.com/89880015/150660246-7721afaf-8b8a-43fe-9023-aeb12a7b947e.png)

3.) Determine the number of unique values for each column.

![image](https://user-images.githubusercontent.com/89880015/150660260-b390885b-cfcb-41e5-a776-2e04be9ee931.png)

4.) For those columns that have more than 10 unique values, determine the number of data points for each unique value.

![image](https://user-images.githubusercontent.com/89880015/150660282-da2950a4-f799-44f7-964a-ce0ec6300a46.png)

5.) Create a density plot to determine the distribution of the column values.

![image](https://user-images.githubusercontent.com/89880015/150660287-61f56765-ba55-4565-baf3-5d6fb4bbb12a.png)

6.) Use the density plot to create a cutoff point to bin "rare" categorical variables together in a new column, Other, and then check if the binning was successful.

![image](https://user-images.githubusercontent.com/89880015/150660326-5826164a-14fc-4ee2-84c0-7b5a1f726e9c.png)

7.) Generate a list of categorical variables.

![image](https://user-images.githubusercontent.com/89880015/150660342-c203bcac-18b1-457b-a3fd-d04343a4c3c2.png)

8.) Encode categorical variables using one-hot encoding, and place the variables in a new DataFrame.

![image](https://user-images.githubusercontent.com/89880015/150660349-6bd77404-356a-4dc4-8bda-cfb71076c18e.png)

9.) Merge the one-hot encoding DataFrame with the original DataFrame, and drop the originals.

![image](https://user-images.githubusercontent.com/89880015/150660603-a94fcec1-bc87-4ccd-bbae-9a24fd2d47c9.png)

# Deliverable 2: Compile, Train, and Evaluate the Model

1.) Continue using the AlphabetSoupCharity.ipynb file where you’ve already performed the preprocessing steps from Deliverable 1.

2.) Create a neural network model by assigning the number of input features and nodes for each layer using Tensorflow Keras.

![image](https://user-images.githubusercontent.com/89880015/150660843-5b605e5f-bd90-447c-bdfa-876e093878a2.png)

3.) Create the first hidden layer and choose an appropriate activation function.

check image on part 3 

4.) If necessary, add a second hidden layer with an appropriate activation function.

check image on part 3 

5.) Create an output layer with an appropriate activation function.

check image on part 3 

6.) Check the structure of the model.

check image on part 3 

![image](https://user-images.githubusercontent.com/89880015/150660911-814d6d57-66c4-437b-a6af-6956c06636cd.png)

7.) Compile and train the model.

![image](https://user-images.githubusercontent.com/89880015/150660925-ad89910b-83d9-40bf-a6a3-adcf040f4226.png)

8.) Create a callback that saves the model's weights every 5 epochs.

9.) Evaluate the model using the test data to determine the loss and accuracy.

![image](https://user-images.githubusercontent.com/89880015/150660954-3d1f55f6-914c-45c2-8c49-bf85ef96bbd4.png)

10.) Save and export your results to an HDF5 file, and name it AlphabetSoupCharity.h5.

![image](https://user-images.githubusercontent.com/89880015/150660976-d4c930df-ceca-4b0b-adf5-912a8efa9ab0.png)

