# Titanic-Survival-Prediction
The Titanic Disaster of 1912 remains one of the most tragic shipwrecks in history, with only around 38% of passengers surviving. The objective of this project is to build a Machine Learning model that can predict whether a passenger would survive or not based on key attributes such as age, gender, passenger class, ticket fare, and family details.

We use Random Forest Classifier, a powerful ensemble learning algorithm, to train our model and achieve high accuracy in predictions.

🎯 Project Objectives
✔ Analyze the Titanic dataset to understand survival trends
✔ Preprocess and clean data for better model performance
✔ Build and train a machine learning model using Random Forest Classifier
✔ Evaluate model accuracy and performance metrics
✔ Deploy a predictive system for real-time survival predictions

🛠 Data Preprocessing & Feature Engineering
Since raw data contains missing values and categorical variables, several preprocessing steps were performed:

1️⃣ Handling Missing Values
Age: Missing values filled using median age per passenger class
Embarked: Missing values replaced with most frequent category (S)
Cabin: Created a new feature Has_cabin (1 = Has Cabin, 0 = No Cabin)
2️⃣ Encoding Categorical Features
Sex → Converted into 0 (Female) and 1 (Male)
Embarked → One-hot encoded into three binary columns (Embarked_C, Embarked_Q, Embarked_S)
Title (extracted from passenger name) → Categorized as Mr, Mrs, Miss, Rare
3️⃣ Feature Engineering
FamilySize = SibSp + Parch + 1 (total family members aboard)
IsAlone = 1 if FamilySize = 1, otherwise 0
FareBin = Categorized ticket fare into groups
AgeBin = Categorized age into groups

Model Performance Metrics
The trained Random Forest Classifier achieved:
✅ Accuracy: 87%
