# Neural_Network_Charity_Analysis

## Analysis Overview
The purpose of this project was to use deep-learning neural network in conjunction with the TensorFlow platform in Python in order to analyze and classify the success of charitable donations. We used the following methods for the analysis:
- preprocessing the data for the neural network model,
- compile, train and evaluate the model,
- optimize the model's performancee.

## Resources
- Data Source: [charity_data.csv](https://github.com/skomyshan/Neural_Network_Charity_Analysis/blob/main/resources/charity_data.csv)
- Software: Python, Anaconda, Conda, Jupyter Notebook

## Results

### Data Preprocessing
- We remove the columns `EIN` and `NAME` because they are identification information and serve no purpose in the input data.
- We designate the column `IS_SUCCESSFUL` as the target for our deep learning neural network because it contains binary data refering to whether or not a charity donation was used effectively.
- We designate the following columns as the features for our model, `APPLICATION_TYPE`, `AFFILIATION`, `CLASSIFICATION`, `USE_CASE`, `ORGANIZATION `, `STATUS`, `INCOME_AMT`, `SPECIAL_CONSIDERATIONS`, and `ASK_AMT`. The categorical variables are encodes, split into training and testing datasets and the features have been standardized.

### Compiling, Training, and Evaluating the Model
- This deep-learning neural network model is composed of two hidden layers awith 80 and 30 neurons.
- To speed up the training process, we used the activation function `ReLU` for the hidden layers. We also used `tanh`.
- Model accuracy is under 75%.

### Summary
The deep-learning neural network model did not achieve the target of 75% accuracy, therefore, we can say that the model is not outperforming. We can opt to use a supervised machine learning model such as the RandomForestClassifier where we can combine multiple decision trees in order to generate a classified output.
