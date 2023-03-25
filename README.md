# Mid-Bootcamp-Project


# Beer Reviews Ratings
**Luciano Sabbatini**  
**IronHack, Germany 24 Mar 2023**

## Goals

* To create a model to predict overall score. 
* Create a standard to rank the beer styles scores in order to be able to recommend beer styles.

Used:

	* Python
	* Statistical analysis
	* Data visualization
	* Jupyter Notebook
	* Tableau
	* Machine Learning (Linear Regression)
  
  ## Data Preparation

### Overview: 
* Dataset is about the ratings, from 1 to 5, of beer tasting reviews:
	* Dataset source: https://www.kaggle.com/datasets/thedevastator/1-5-million-beer-reviews-from-beer-advocate
  
* 14 columns 
* 1586614 rows 
* columns:
 
| Initial Column | Description | 
| --- | --- |
| brewery_id | Unique identification of the brewery | 
| brewery_name | Name of the brewery |
| review_time | Unique time when review was made |
| review_overall | Based on|all factors, the final score |
| review_aroma | Rating based on how the beer smells |
| review_appearance | Rating based on how the beer looks | 
| review_profilename | Reviewer’s user ID |
| beer_style | Category of the beer |
| review_palate | Rating based on how the beer interacts with the|  palate| || |
| review_taste | Rating based on how the beer actually tastes|  |
| beer_na|e | Name of the beer |
| beer_abv | Alcohol by volume |
| beer_beerid | Unique beer identification |

 
### Data Wrangling and Cleaning
  
- Dropping rows of nulls, filling nulls
- Deleting  columns with identifier id on it 
- Converting UNIX time into datetime
- Analysing unique features of the dataset 
- Analysing the relations between the sensorial factors and oberall ratings ratings
- Creating plots for better visualization
- Creating new columns
- Creating Step conclusions for each part of the analysis
- Building a recommendation system
- Testing the model.

## Data Analysis
* Use [tableau][(https://public.tableau.com/app/profile/luciano.sabbatini/viz/beerproject_visualization/Dashboard1?publish=yes)]


### Data Exploration and Visualization
Used Python and Tableau to visualize my overall data.

### Model Training and Evaluation
- Define predictors and target values (X, y)
- Standard scaling for numericals : for Train and Test set
- Models : LinearRegression, MLPRegressor & KNN neighbors
- Compared accuracy 

## Conclusion

1) Our dataset features were insufficient to create a usefull model to predict overall ratings. The ratings are indivudual unique caracheteristics and in order to build a machine learning model the dataset would need to have the components of each beer for instance.
2) Through confidence intervals on the overall ratings on beer styles, we were able to classify and have a reliable system to recommend beer styles.
