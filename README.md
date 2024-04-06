This repository contains code for predicting heart disease using machine learning algorithms. The dataset used for training and testing the models is available in the heart.csv file. Various classification algorithms such as Random Forest, Support Vector Machine (SVM), Decision Tree, K Nearest Neighbors (KNN), and Logistic Regression have been implemented and evaluated for their performance.

Dependencies:

Ensure you have the following dependencies installed to run the code:

Python 3:

pandas
seaborn
matplotlib
scikit-learn
numpy
Usage
Clone this repository to your local machine.
bash

git clone <repository_url>
Navigate to the directory containing the code.
bash

cd <repository_directory>
Run the code using a Python environment.

python heart_disease_prediction.py
Data

The dataset used for heart disease prediction is available in the heart.csv file. It contains the following columns:

age: Age of the patient
sex: Gender of the patient (0 = female, 1 = male)
cp: Chest pain type (0 = typical angina, 1 = atypical angina, 2 = non-anginal pain, 3 = asymptomatic)
trestbps: Resting blood pressure (in mm Hg)
chol: Serum cholesterol (in mg/dl)
fbs: Fasting blood sugar > 120 mg/dl (1 = true, 0 = false)
restecg: Resting electrocardiographic results (0 = normal, 1 = having ST-T wave abnormality, 2 = showing probable or definite left ventricular hypertrophy)
thalach: Maximum heart rate achieved
exang: Exercise-induced angina (1 = yes, 0 = no)
oldpeak: ST depression induced by exercise relative to rest
slope: Slope of the peak exercise ST segment (0 = upsloping, 1 = flat, 2 = downsloping)
ca: Number of major vessels (0-3) colored by fluoroscopy
thal: Thalassemia (0 = normal, 1 = fixed defect, 2 = reversible defect)
target: Presence of heart disease (1 = yes, 0 = no)

Results:

A visualization of the distribution of target values (presence/absence of heart disease) is plotted using seaborn and matplotlib.
Missing values in the dataset are checked and displayed using data.isnull().sum().
Basic information about the dataset is printed using data.info().
Descriptive statistics of the dataset are displayed using data.describe().
Box plots for each feature are visualized to identify outliers.
Outliers in specific features (e.g., 'trtbps', 'chol', 'oldpeak', 'caa') are handled by replacing them with median values.
A correlation matrix heatmap is plotted using seaborn to identify relationships between features and the target variable ('output').
Classification algorithms including Support Vector Machine (SVM), Decision Tree, K Nearest Neighbors (KNN), Random Forest, and Logistic Regression are implemented and evaluated for accuracy.
The variation of accuracy with the number of neighbors (for KNN) and the number of estimators (for Random Forest) is visualized using line plots.
Contact
For any questions or feedback, please contact Omar Salman.
