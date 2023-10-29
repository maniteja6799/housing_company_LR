# Housing_company Linear regression

Dataset of a Housing company is shared. This is an attempt to understand the data, create a linear regression model to determine the impact of measured metrics over the period. 

## Table of Contents

- [General Information](#general-information)
- [Data characteristics](#dataset-characteristics)
- [Conclusions](#conclusions)
- [Technologies Used](#technologies-used)
- [Contact](#contact)

## General Information

This project is to create a regularised linear regression model to the provided Housing dataset to find out various parameters which could affect the sale price for houses.

Following EDA and Data transformations applied before the model creation:

- Pair-plot on dependant and independent vars to identify their relationships
- Dropped columns, Transformed variables
- Box plots on categorical variables, distribution plots for variables
- Creating mappings for for categorical vars
- Splitting data to train and test
  

## Dataset characteristics

Dataset contains a total of ~1.5 entries with 81 columns. 43 of them are categorical and the rest continuous. 


## Conclusions

### Insights from EDA

1. `LotFrontatge` has too many null variables and doesn't have much correlation with the dependant variable..
2. `SalesPrice` is skewed towards one side. Log distribution is much more normal and it's better to predict that.
3. Living area and Basement area size seem to have a positive linear relation with target variable.
4. If there is an alley present, A paved alley on average has a better sale price than gravel alley.


### Predicted models 

- A simple unregularised model gave a 0.88 test r2 score
- Adding a lasso regularisation increased it to 0.91 with alpha at 0.0007
- OverallQual(0.77) and GrLivArea(0.72) are the most significant variables.

## Technologies Used

- Python 3.10.9
- Jupyterlab 3.6.3
- numpy 1.23.5
- pandas 1.5.3
- matplotlib 3.7.0
- seaborn 0.12.2

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->


## Contact

Created by [Pawan Mani Teja Kuppili](https://github.com/maniteja6799)