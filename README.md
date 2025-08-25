# forest_cover_type

This notebook focuses on Forest Cover Type Classification using the covtype.csv dataset, which contains 581,012 data points and 55 features.

Here's a brief overview of the steps taken:

📊 Data Loading and Exploration: Loaded the dataset and performed initial exploration to understand its structure and features. Identified and removed 4 columns with very low standard deviation.

🌳 Handling Imbalanced Data: Noticed a significant class imbalance in the 'Cover_Type' distribution, with the smallest class having 2,747 samples. Addressed this by implementing Undersampling to balance the classes for training, resulting in a dataset of 19,229 samples.

🛠️ Feature Engineering: Converted the one-hot encoded 'Wilderness_Area' and 'Soil_Type' features back into single categorical columns to potentially improve model performance.

🤖 Model Training and Evaluation: Trained several classification models on the undersampled data, including:

Logistic Regression
Decision Tree Classifier
Random Forest Classifier
XGBoost Classifier
Gradient Boosting Classifier
Evaluated each model using accuracy, confusion matrix, and classification report to assess their performance on the undersampled dataset. The Random Forest Classifier achieved an accuracy of 86.65% and the XGBoost Classifier achieved an accuracy of 86.43% on the undersampled test set.
