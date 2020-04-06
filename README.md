# Wine Review - analysis

The aim of this analysis is to understand where the quality wine comes from, what is the correlation between the score and the price or the vintage of the wine and finally, classification model is bulit to predict whether the wines quality is above or below average. Initial work included exploring the data, removing duplicate rows, imputing missing values and finally discarding some observations. 

------

### Medium post


------

### The analysis

#### 1. Where does the quality wine come from?

* ratings by average score show that England has the best quality wine
* somehow surprising result could be due to samle size (only 63 English wines in dataset)
* ratings by maximum score show that Italy, Portugal, US, France and Australia are in the lead. 
* US has the biggest spread of scores, but it's expected since wines from this country make up for 40% of the dataset

#### 2. More expensive the wine the better quality it is - Truth or myth?

* truth in most cases, average score increases when the price of the wine increases
* however, price is not the only indicator of wines quality since the bottle for $4 from US scores only 2 points less than bottle from France for $3300.

#### 3. How to choose good quality wine wisely?

* there is a correlation between price and score: 0.4
* there is no correlation between vintage and score/price
* the strongest correlation is between description length and score: 0.6

#### 4. Can predictive model identify the quality of wine?

* model predicts whether the wine is better or worse than a treshold (here - average score)
* the random forest model scored 58% better than a well_informed random guess.
* accuracy: 84.12%

------

### Libraries used:
* numpy
* pandas
* scipy
* matplotlib
* seaborn
* nltk
* collections
* re
* sklearn
* wordcloud

------

### Repository files:
* wine_project_-_cleaning_data.ipynb - Jupyter notebook with initial exploration and data cleaning
* wine_project_-_model_fitting.ipynb - Jupyter notebook with fitting the model
* wine_project_-_visualisations.ipynb - Jupyter notebook with visual analysis

------

### Acknowledgments
* Data source: https://www.kaggle.com/zynicide/wine-reviews
