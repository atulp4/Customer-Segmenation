# Customer-Segmenation

## Business Problem 

The credit card business of a large conglomerate is interested in acquiring new customers from its movie customer base. The goal is to identify and target profitable customers from the movie business who have potential to purchase the credit cards.

## Data

The raw data contains transactional information of VOX customers over a period of 1 year across 26 cinema locations. 

**Data Cleaning:**
- Removed duplicate records
- Dropped columns with >90% missing values 
- Imputed missing values using KNN imputer
- Formatted data types

After cleaning, the final dataset contains 22,488 customers and 53 variables related to their movie watching behavior, spending patterns, preferred movie types, booking channels etc.

## Analytics Approach

The project follows a standard data science lifecycle:

**Data Understanding:**
- Created a data dictionary to document all variables
- Analyzed distribution of variables, identified outliers
- Calculated summary statistics on the data

**Feature Engineering:**
- Removed highly correlated variables using correlation matrix and VIF
- Imputed missing values using KNN imputer
- Generated new features like average spend per visit and customer tenure 

**Model Building:**
- Compared performance of Logistic Regression, KNN, Random Forest models
- Tuned hyperparameters using RandomizedSearchCV
- Evaluated models using AUC, recall, precision metrics

**Model Evaluation:**
- Logistic Regression and KNN had lower AUC scores around 54-55%
- Random Forest performed best with AUC of 58% and recall of 78%
- Selected Random Forest as the final model based on business requirement of maximizing recall.

## Notes

In this project the following were accomplished - 

1. Contextualized problem statement definition can be found in

         - Customer_Segmentation_VOX.pdf

2. Understood the dataset

         - Dataset Summary.xlsx

3. Generated data dictionary after cleaning the dataset

         - Data Dictionary - After Cleaning .xlsx

4. Peformed Factor Mapping and Hypothesis testing

         - Factor Mapping and Hypothesis.xlsx

5. Consecutively performed EDA including Univariate and Bivariate analysis
    
          - Bivariate Analysis.xlsx

6. Conducted feature extraction

          - Feature_extraction_bivariates.xlsx

7. Checked correlation between variables

          - Correlation Matrix.xlsx

8. Picked out highly correlated variables

          - Highly_corr_cols.xlsx

9. Checked viability of variables and selected the appropriate features

          - VIF_Data.xlsx & VIF_Iterations.xlsx

10. Fit different models

          - Modelling Iterations.xlsx

11. Code used for this project

          - Segmentation_Code_Snippet.ipynb

12. The capstone project included presentations of different stages of the solution which were divided into three reviews : 

          - Review 1 - Capstone Project - NAJM - Final Deck.pdf
          - Review 2 - Capstone Project - NAJM - Final Deck.pdf
          - Review 3 - Capstone Project - NAJM - Final Deck.pdf
   
13. Wrote a paper and submitted to the university for final year practicum (graded)

          - Customer_Segmentation_PAPER.pdf 



