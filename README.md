# Mid-Bootcamp-Project
Dataset source: https://www.kaggle.com/datasets/thedevastator/1-5-million-beer-reviews-from-beer-advocate

# Credit-Card-Fraud-Detection-Project
**Meysour Omezzine**  
**IronHack, Paris 21 Mar 2023**

## Overview

* How we can Banks/Credit card companies predict fraudulent credit card transactions?  

Used:

	* Python
	* Statistical analysis
	* Data visualization
	* Jupyter Notebook
	* Tableau
	* Machine Learning (Logistic Regression)
  
  ## Data Preparation

### Overview: 
* Data is about Credit card transactions.
	* [dataset](https://www.kaggle.com/datasets/ealtman2019/credit-card-transactions)
  
* 15 columns 
* 19963 rows 
* columns:
* 
| Initial Column | Comments | New Column |
| --- | --- | --- |
| User | User is just an index not an ID | None : Dropped |
| Card | No further infos about this column | Card |
| Year | Added to Date column | Date |
| Month | Nothing to edit | Month |
| Day | Added to Date column | Date |
| Time | Binned to 4 categories and added to Time Period | Time & Time_Period |
| Amount | Binned to 3 categories | Amount & Amount_Range |
| Use chip | Nothing to edit | Use Chip |
| Merchant name | Too many unique values. | None:Dropped |
| Merchant City | Changing Merchant City to Merchant Type : Online or In-person | Merchant Type |
| Merchant State | Binned to 4 main catgories | Merchant_State_grouped |
| Zip | Too many unique values, gives same indication as Merchant City | None: Dropped |
| MCC | Changing MCC to MCC Category: Check for each MCC number Category name and group same categories fields together | MCC_Category |
| Errors? | Binned | Errors? |
| Is Fraud? | Main target | Is Fraud? |

 
### Data Wrangling and Cleaning
  
- Overall Data description
- Deleting  columns with hight unique values: User,Merchant Name,Zip 
- Looking for outliers column by column 
- Dealing with Nan Values for each column
- Creating plots for each column to check where most fraudulent transactions occured
- Checking for correlation with target feature


### Data Storage

* Dump your data as `.csv` file. 

## Data Analysis
* Use [tableau](https://public.tableau.com/app/profile/omezzine.meysour/viz/Creditcardfraudanalysis_16794785656020/Fraudsbyamount?publish=yes) to analyze 


### Data Exploration and Visualization
Used Tableau to visualize my overall data.

### Model Training and Evaluation
- Define predictors and target values (X, y)
- Standard scaling for numericals : for Train and Test set
- OneHotEncoding for categoricals : for Train and Test set
- Balancing data : Oversampling our target values in our Train set. 
- Models : LogisticRegression & KNN neighbors
- Compared accuracy 
- Confusion Matrix

## Conclusion

- Based on our Recall rate, our model can alert us on fraud transactions where transactions are actually frauds, how ever based on the confusion matrix it predicted some false positives. 
- Our model had an accuracy of 89%. 
