# Heart Failure Prediction

**Overview:**
This project focuses on developing a predictive model to determine the likelihood of an individual having heart disease based on various health-related features. The dataset used for training and evaluation contains information such as age, sex, chest pain type, resting blood pressure, cholesterol levels, fasting blood sugar, resting electrocardiographic results, maximum heart rate achieved, exercise-induced angina, oldpeak, and the slope of the ST segment.

**Data Source:**
The dataset was obtained from Kaggle, a renowned platform for data science competitions and datasets. The dataset provides a valuable resource for exploring and understanding factors contributing to heart disease and enables the development of predictive models to assist in early detection.
Link for the dataset https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction

**Data Exploration and Preprocessing:**

- The dataset is loaded into a Pandas DataFrame, and an initial exploration is conducted to understand the structure and content.
- Data cleaning involves handling missing values and removing records with unusual resting blood pressure values.
- Categorical variables are processed, and values are encoded for use in machine learning models.

**Exploratory Data Analysis:**

- Outliers are visualized using box plots to understand the distribution of key features.
- Duplicates in the dataset are identified and addressed.

**Feature Engineering:**

- The 'FastingBS' feature is transformed to replace numeric values with more meaningful labels ('Normal' and 'Prediabetes').
- Feature selection is performed, and the independent and dependent variables are defined.

**Model Development:**

- The dataset is split into training and testing sets using the train_test_split function.
- A preprocessing pipeline is defined, which includes handling missing values, scaling numeric features, and encoding categorical features.
- The Random Forest Classifier is chosen as the predictive model due to its effectiveness in handling complex datasets and providing robust predictions.
- The model is trained using the training set, and predictions are made on the test set.

**Model Evaluation:**

- The performance of the model is assessed using metrics such as accuracy, classification report, and cross-validation scores.
- Cross-validation is employed to ensure the generalizability of the model to new data.

**Model Export:**

- The trained model is saved using the joblib library for future use.
- Feature names are stored in a JSON file ('features.json') to maintain transparency and facilitate understanding.

**Conclusion:**
This project provides a comprehensive solution for predicting heart disease based on a set of health-related features. The developed model demonstrates strong predictive performance, and the exported artifacts (model and feature information) can be used for deployment in real-world scenarios. The combination of exploratory data analysis, feature engineering, and machine learning techniques contributes to a robust and reliable predictive model for heart disease detection.

**Model Utilization:**

- The trained model is loaded for practical use.
- A user-friendly prediction function is developed, allowing users to input specific health-related features to predict the likelihood of heart disease.
- The function includes loading the necessary model, scaler, and column information.
