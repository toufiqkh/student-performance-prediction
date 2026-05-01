Student Performance Prediction Project

**Problem Statement**
The purpose of this project is to analyze student exam performance and build a model that can predict scores. Alongside prediction, the project identifies the main factors that influence student outcomes, such as gender, parental education, lunch type, and test preparation.

**Data Cleaning** 	
•	Checked the dataset for missing values → none were found.
•	Converted categorical variables (gender, lunch, parental education, etc.) into numerical codes using one-hot encoding.
•	Verified that all numeric columns (math, reading, writing scores) were properly formatted.

**Feature Engineering (Average Score)**
A new column was created: Average Score = (Math + Reading + Writing) / 3
This allowed us to evaluate overall performance instead of focusing only on individual subjects.

**EDA Insights **
1.	Gender Impact: Female students scored higher in reading and writing, while male students performed better in math.
2.	Parental Education: Students with parents holding bachelor’s or master’s degrees achieved higher average scores compared to those with only high school education.
3.	Lunch Type: Students with standard lunch consistently outperformed those with free/reduced lunch.
4.	Test Preparation: Completing a test preparation course had a clear positive effect on scores.
5.	Correlation Between Subjects: Reading and writing scores were strongly correlated, showing that students who excelled in reading usually did well in writing too.

**Model Used**
•	Linear Regression was applied to predict average scores.
•	For comparison, Decision Tree Random Forest models were also tested.

**Evaluation Metrics**
•	Mean Absolute Error (MAE): Measures the average prediction error.
•	Root Mean Square Error (RMSE): Penalizes larger errors more strongly.

**Results:**
•	Linear Regression gave stable predictions.
•	Linear Regression -> MAE: 10.49, RMSE: 13.40
•	Random Forest performed slightly better, capturing complex relationships in the data.
•	Random Forest -> MAE: 11.48, RMSE: 14.78
•	Decision Tree was less consistent compared to Random Forest.
•	Decision Tree -> MAE: 11.88, RMSE: 15.25

**Key Factors Affecting Performance**
•	Completion of test preparation courses
•	Lunch type (standard vs free/reduced)
•	Parental education level
•	Gender differences in subject strengths

**Final Conclusion**
This project demonstrates that student performance is influenced by both academic preparation and socio-economic factors. While ability matters, external support such as parental education, proper nutrition, and preparation courses significantly improve outcomes.
The models built can predict scores and highlight areas where interventions (like providing better lunch or preparation support) can help students perform better. Random Forest gave the most accurate predictions, but Linear Regression remains a simple and effective baseline model.










