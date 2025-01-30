# Module-21-deep-learning-challenge
Assignment 21 - deep-learning-challenge

**1. Overview**: The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

**2. Results:**

o	Data Preprocessing
What variable(s) are the target(s) for your model? Target variable = IS_SUCCESSFUL -- 1 is considered yes (successful) and 0 is considered no (not successful)
What variable(s) are the features for your model? Features = there are 9 features - all the other columns
What variable(s) should be removed from the input data because they are neither targets nor features? 'EIN', 'NAME'- non-beneficial ID columns

o	Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why?
Were you able to achieve the target model performance?
What steps did you take in your attempts to increase model performance?

**3. Summary**

**PREPROCESSING THE DATA BY**:

dropping non-beneficial columns,
finding the number of data points for each unique value for each of the columns that had more than 10 unique values - APPLICATION_TYPE and CLASSIFICATION,
choosing a cutoff point of 600 and 300, respectively, to bin rare categorical values together into a new value called "Other",
using pd.get_dummies() to convert categorical data to numeric,
dividing the data into a target array (IS_SUCCESSFUL) and features arrays,
applying the train_test_split to create a testing and a training dataset,
and finally, using StandardScaler to scale the training and testing sets
The resulting data included 44 features. The target variable (y) was IS_SUCCESSFUL. The data was split into training and test subsets.

**COMPILING, TRAINING, AND EVALUATING THE MODEL**
The result in the accuracy around 72%, so a little short of the required target accuracy.
