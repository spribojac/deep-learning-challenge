# deep-learning-challenge
Module 21 Neural Networks and Deep Learning

# Deep Learning Challenge: Alphabet Soup Charity
## Overview of the Analysis:
The goal of this project is to create a binary classifier using deep learning to predict the success of organizations funded by Alphabet Soup. The provided dataset contains information about over 34,000 organizations that have received funding, including various features such as application type, affiliation, classification, and income. The challenge involves preprocessing the data, designing a neural network model, and optimizing it to achieve a predictive accuracy higher than 75%.

### Files:
Starter Files: Module 21 Challenge files

Results File: AlphabetSoupCharity.h5

Optimized Model File: AlphabetSoupCharity_Optimization.h5

Report File: Report.md

## Step 1: Preprocess the Data
1. Load and Explore Data:
  - Read in the charity_data.csv to a Pandas DataFrame.
  - Identify the target variable(s) and feature(s).
  - Drop the EIN and NAME columns.
2. Data Exploration:
 - Determine the number of unique values for each column.
 - For columns with more than 10 unique values, analyze the number of data points for each unique value.
 - Bin "rare" categorical variables together in a new value, "Other."
3. Encoding Categorical Variables:
 - Use pd.get_dummies() to encode categorical variables.
4. Train-Test Split:
 - Split the data into features array (X) and target array (y).
 - Use train_test_split to split the data into training and testing datasets.
5. Scale Features:
 - Use StandardScaler to scale the training and testing features datasets.

## Step 2: Compile, Train, and Evaluate the Model
1. Neural Network Model:
 - Design a neural network model using TensorFlow and Keras.
 - Choose the number of input features, nodes for each layer, and appropriate activation functions.
 - Check the structure of the model.
2. Compile and Train:
 - Compile the model.
 - Train the model, creating a callback to save weights every five epochs.
3. Evaluate Model:
 - Evaluate the model using the test data to determine loss and accuracy.
 - Save and export results to AlphabetSoupCharity.h5.

## Step 3: Optimize the Model
1. Exploratory Data Analysis:
 - Adjust input data to eliminate confusion.
 - Modify column selections, bin sizes, or values to enhance model performance.
2. Model Optimization:
 - Adjust model architecture:
 - Add more neurons or hidden layers.
 - Use different activation functions.
 - Change the number of epochs in training.
3. Export Optimized Model:
 - Save and export optimized results to AlphabetSoupCharity_Optimization.h5.

## Step 4: Write a Report on the Neural Network Model
### Data Preprocessing
- Target Variable(s): IS_SUCCESSFUL
- Feature Variable(s): All columns except EIN and NAME.
- Remove Variables: EIN, NAME

### Compiling, Training, and Evaluating the Model
#### Model Architecture:
- Input Layer: Number of features
- Hidden Layers: Number of neurons and appropriate activation functions
- Output Layer: Binary classification activation function
#### Model Performance:
- Achieved target model performance.
- Steps taken to increase performance.

## Summary
The deep learning model successfully predicts the success of organizations funded by Alphabet Soup. The model architecture and preprocessing steps were crucial in achieving the target performance. Further exploration and adjustments were made for optimization. The recommendation for a different model would depend on the specific dataset characteristics and problem requirements.

## Step 5: Copy Files Into Your Repository
1. Download Files: Download Colab notebooks to your computer.
2. Move to Repository: Move files into the Deep Learning Challenge directory in your local repository.
3. Push to GitHub: Push added files to GitHub.

## Credits
Thanks to @jojoalva for help with this one! Teamwork makes the dreamwork
