## Model Report

Overview of the analysis: Explain the purpose of this analysis.
With our new machine learning and neural networks skills, using the dataset provided, we created a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

Data Preprocessing
1.Drop the EIN and NAME columns.
2.Determine the number of unique values for each column.
3.For columns that have more than 10 unique values, determine the number of data points for each unique value.
4.Use the number of data points for each unique value to pick a cutoff point to combine "rare" categorical variables together in a new value, Other, and then check if the replacement was successful.
5.Use pd.get_dummies() to encode categorical variables.
6.Split the preprocessed data into a features array, X, and a target array, y. Use these arrays and the train_test_split function to split the data into training and testing datasets.
7.Scale the training and testing features datasets by creating a StandardScaler instance, fitting it to the training data, then using the transform function.

What variable are the target for your model?
The target variable is the 'IS_SUCCESSFUL'.

What variable should be removed from the input data because they are neither targets nor features?
'EIN' and 'NAME' columns were dropped from the dataset .

Were you able to achieve the target model performance?
After three attempts, I was not. The highes performance I was able to achieve was 73%.

What steps did you take in your attempts to increase model performance?
I added more hidden layers, added more neurons to a hidden layer, drop more columns, changes the activation function, reduce the number of epochs to the training regimen and change de bin.

After multiple attempts< I was not able to achieve 75% accuracy on any of the models. I do not recommend this model for the initial purpose since the accuracy is too low. In order to improve it, I would recommend to filter the data more thoroughly and try creating different layers. 