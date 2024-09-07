# CrimeCast-Forecasting-Crime-Categories-IITM
This project includes analysis of a dataset filled with information about crime incidents. The goal is to use the data to predict the type of crime that occurred after looking the incidents happened, details about the victims, and other important factors.  

**Table of Contents**

1. Getting Started
2. Data Description
3. Exploratory Data Analysis (EDA)
4. Feature Engineering
5. Modeling
6. Results

**Data Description**

- Location: Street address of the crime incident.
- Cross_Street: Cross street of the rounded address.
- Latitude: Latitude coordinates of the crime incident.
- Longitude: Longitude coordinates of the crime incident.
- Date_Reported: Date the incident was reported.
- Date_Occurred: Date the incident occurred.
- Time_Occurred: Time the incident occurred in 24-hour military time.
- Area_ID: LAPD's Geographic Area number.
- Area_Name: Name designation of the LAPD Geographic Area.
- Reporting_District_no: Reporting district number.
- Part 1-2: Crime classification.
- Modus_Operandi: Activities associated with the suspect.
- Victim_Age: Age of the victim.
- Victim_Sex: Gender of the victim.
- Victim_Descent: Descent code of the victim.
- Premise_Code: Premise code indicating the location of the crime.
- Premise_Description: Description of the premise code.
- Weapon_Used_Code: Weapon code indicating the type of weapon used.
- Weapon_Description: Description of the weapon code.
- Status: Status of the case.
- Status_Description: Description of the status code.
- Crime_Category: The category of the crime (Target Variable)

**Exploratory Data Analysis (EDA)**

We perform various EDA tasks to understand the dataset better:

- Visualizing the distribution of categorical variables like Victim_Sex, Crime_Category, Status, and Victim_Descent.
- Analyzing the number of crimes reported over time to identify trends.
- Plotting the number of crimes by location and examining the relationship between victim age and crime count.

**Feature Engineering**
To improve model performance, we:

Dropped redundant columns with high correlation.
Handled date features by extracting useful components like year, month, day, and weekday.
Managed missing values and scaled numerical features.
Processed categorical features with one-hot encoding and text features with TF-IDF vectorization.
Modeling

**We implemented and evaluated several machine learning models:**
Logistic Regression: Used for its simplicity and effectiveness in binary classification tasks.
Random Forest Classifier: A robust model for handling large datasets and complex relationships.
XGBoost: Known for its high performance in classification tasks.
Each model was tuned using GridSearchCV to find the best hyperparameters and evaluated based on accuracy, precision, recall, and F1-score.

**Results**

The models performed well, with precision, recall, and F1-score values greater than 0.80. The final selected model achieved an accuracy of approximately 83% on the validation set.

