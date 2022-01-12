# Genetics-Capstone-3
Third Capstone project for Springboard 

## Problem Statement:

With the exponential increase in world population, there is a correlating increase in genetic mutations that lead to a range of genetic defects in a range from mild to fatal. Hereditary illnesses are becoming more common due to a lack of understanding about the need for genetic testing. Often kids die as a result of these illnesses, thus genetic testing is critical for individuals interested in becoming parents to understand risks of genetic disorders that are present in their own DNA and that can be passed on. This therefore leads to the question, can these hereditary illnesses be predicted? 


Using a dataset from Kaggle.com, which included demographic data such as the patient’s age, mother’s age, father’s age, as well as health data such as blood cell count, white blood cell count, respiratory rate, and heart rate. I used this data to create multiple neural networks and tune them with learning rate schedulers to determine if these conditions can be predicted, and with what accuracy they can be predicted. 

## Data Wrangling and Cleaning:
	
For this dataset there were many columns that were unnecessary for a fruitful analysis such as patient name, family name, patient id, location of institute, institute name, father’s name, and place of birth. As these variables were not pertinent to a patient’s health or hereditary they were unnecessary for analysis. There were also a plethora of missing values in the data. I chose to fill the numeric missing values with the median, and for the categorical variables, I filled the majority of categorical variables with a backfill method to keep as much continuity in the data as possible. There were also missing values in the Genetic Disorder and Subclass Disorder columns and since those are the target variables, I dropped the NA values in those columns in order to maintain the data integrity. The final data that I analyzed for the Genetic Disorder neural network consisted of 18,047 data points and 29 columns with Genetic Disorder being the target variable. The final data I analyzed for the Subclass Disorder neural network consisted of 18,047 data points and 30 columns with Subclass Disorder being the target variable.


* Further information and analysis about the report can be found in the Final_report section of this repository
