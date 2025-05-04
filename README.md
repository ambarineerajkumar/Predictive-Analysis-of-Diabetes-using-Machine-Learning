
# 📘 Project Title: Diabetes Prediction Using Machine Learning 

# 📝 Summary
This project explores the use of machine learning algorithms to predict diabetes using a dataset containing patient health indicators. The primary aim is to help in early detection and diagnosis of diabetes by training predictive models. The project workflow includes data preprocessing, visualization, model training, evaluation, and interpretation. The entire workflow was implemented using Python in a JupyterLab environment, with version control managed through Git.

![Diabetes](https://github.com/user-attachments/assets/0dd2d3f0-136e-4873-b321-dadf61d3d15e)

# 🛠️ Tools & Technologies Used


Tool / Library	Purpose

JupyterLab	Development environment for code, markdown, and output

Python	Programming language

Pandas	Data manipulation and analysis

NumPy	Numerical operations

Matplotlib / Seaborn	Visualization of data distributions and relationships

Scikit-learn	ML model building, training, and evaluation

Git	Version control and source tracking

Excel (xlsx)	Source format for the diabetes dataset

# 📊 Analysis Report
📂 Dataset Overview
The dataset consists of 768 records with 8 medical attributes and 1 target variable:

Independent Features: Pregnancies, Glucose, BloodPressure, SkinThickness, Insulin, BMI, DiabetesPedigreeFunction, Age

Target Variable: Outcome (0 = No Diabetes, 1 = Diabetes)

🧹 Data Cleaning
Replaced invalid values (zeros) in features like Glucose, BloodPressure, BMI, etc., with median values.

Handled missing/null values appropriately.

Scaled numerical features using MinMaxScaler.


# 📊 Data Visualization
Heatmap shows high correlation between Glucose, BMI, and Outcome.

Pairplots and histograms indicate clear distribution differences between diabetic and non-diabetic patients.

# 🤖 Model Training
The following models were trained using Scikit-learn:

Model	Accuracy (%)	Key Observation
Logistic Regression	~76%	Good interpretability
Decision Tree	~72%	Overfits slightly on training data
Random Forest	~80%	Best performance, generalizes well
KNN (K=5)	~74%	Sensitive to feature scaling

# 📉 Evaluation Metrics
Confusion Matrix

Precision, Recall, F1-Score

ROC AUC Curve

Random Forest achieved the highest AUC and F1-score, making it the most robust model for this use case.

# ✅ Conclusion
The diabetes prediction model built using machine learning proves to be effective, particularly with the Random Forest Classifier. With proper preprocessing, visualization, and model evaluation, it's possible to derive meaningful insights and predictive power from healthcare data. The project emphasizes the importance of data quality, model selection, and evaluation in developing trustworthy ML systems in healthcare.
