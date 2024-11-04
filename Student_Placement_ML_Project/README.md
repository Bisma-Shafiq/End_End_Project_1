## Project Overview
This project focuses on developing a placement prediction model for students based on their academic performance and IQ. The model predicts whether a student will get placed in a company or not, based on their CGPA and IQ scores.

## Data Description
The dataset contains information on student attributes:
cgpa: The student’s cumulative GPA.
iq: The student’s IQ score.
placement: Target variable indicating placement status (1 for placed, 0 for not placed).
The data undergoes preprocessing and is divided into features (cgpa, iq) and the target (placement).

## Project Workflow
1- Exploratory Data Analysis (EDA):

Scatter plots are used to visualize the relationship between CGPA and IQ based on placement status.
cgpa and iq serve as features for input, and placement is used as the output label.
Data Splitting:

The data is split into training and testing sets using an 90-10 split.

2- Data Scaling:

Features are standardized using StandardScaler to bring them to a similar scale, improving model performance.

3- Model Training:

A logistic regression model is trained to predict placement.
Model coefficients and intercepts are analyzed to understand the influence of each feature on placement probability.

4- Model Evaluation:

Predictions are generated on the test set, and accuracy is calculated to evaluate model performance. In this project, an accuracy of 80% is achieved on the test data.
Decision Boundary Plotting:

The decision boundary for the logistic regression model is visualized using the mlxtend.plotting.plot_decision_regions function, helping in understanding how well the model separates placed and non-placed students.

5- Model Deployment:

The trained logistic regression model is saved as a pickle file (PlacementModel.pkl) for deployment and future use.

## Dependencies
pandas for data manipulation
numpy for numerical operations
matplotlib and seaborn for data visualization
sklearn for machine learning algorithms and utilities
mlxtend for plotting decision boundaries
pickle for model serialization

## Usage
### Load the Model:

The trained model (PlacementModel.pkl) can be loaded in a Python environment using pickle to make predictions on new data.
Prediction:

Input CGPA and IQ scores to predict the placement status using the loaded logistic regression model.
## Results
The model achieves an accuracy of 80%, indicating it effectively differentiates between students who are likely to get placed and those who aren’t. This tool can be useful for educational institutions and students to understand the likelihood of placement based on academic performance and cognitive ability.
