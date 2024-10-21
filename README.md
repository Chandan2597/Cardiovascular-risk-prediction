The objective of this project is to utilize machine learning techniques to predict the 10-year risk of future coronary heart disease (CHD) in patients, using data from the ongoing Framingham Heart Study, which involves residents of Framingham, Massachusetts. The dataset comprises over 4,000 patients and includes 15 attributes, each representing a potential risk factor for CHD. These attributes encompass demographic, behavioral, and medical factors.

### Data Preparation and Preprocessing
To ensure the dataset's quality and suitability for analysis, extensive preprocessing was conducted. Missing values were handled using median and mode imputation. Outliers were identified and removed using the Interquartile Range (IQR) method. To address skewness in continuous variables, log and square root transformations were applied, improving model performance by normalizing the data distribution.

### Feature Engineering and Selection
To enhance the dataset, feature selection was carried out using the Variance Inflation Factor (VIF) to eliminate multicollinearity. A new feature, pulse pressure, was created to capture the relationship between systolic and diastolic blood pressure. Additionally, redundant columns were removed to streamline the dataset. Key features identified for predicting CHD risk included 'Age', 'Sex', 'Education', 'Cigarettes per day (cigs_per_day)', 'Blood pressure medication (BPMeds)', 'Prevalent stroke', 'Prevalent hypertension (prevalent_hyp)', 'Diabetes', 'Total cholesterol', 'Body Mass Index (BMI)', 'Heart rate', 'Glucose', 'Pulse pressure'.

### Addressing Imbalanced Data
Given the imbalanced nature of the dataset, the Synthetic Minority Over-sampling Technique (SMOTE) combined with Tomek links undersampling was employed to balance the class distribution. This technique improved model performance by ensuring a more equitable representation of classes. Additionally, data scaling was performed using the Standard Scaler method to bring all features onto the same scale.

### Model Evaluation and Selection
Several machine learning models were evaluated based on their recall performance, as the primary objective was to maximize the identification of patients at risk of CHD. After thorough analysis, the tuned Neural Network emerged as the final prediction model due to its superior recall score. Prioritizing recall ensured that as many patients with CHD risk as possible were correctly identified, even at the expense of some false positives.

### Conclusion
This project demonstrates the efficacy of machine learning techniques in accurately predicting CHD risk in patients using data from a cardiovascular study. Through meticulous data preprocessing and transformation, careful feature selection, and choosing an optimal model based on recall performance, it was possible to achieve a positive business impact. Accurately predicting CHD risk can lead to timely interventions and improved patient outcomes, showcasing the potential of machine learning in healthcare.
