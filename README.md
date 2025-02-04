# Module 2 Final Project - Property Development in King County, Washington


## Overview
```
index.ipynb             
# Jupyter notebook containing code for data discovery, EDA and the multivariate linear regression model

presentation.pdf        
# A non-technical presentation of the project findings

kc_house_data.csv       
# Raw dataset of house prices between 2014-15 for King County

zipcode_areas_king_county.geojson
# GeoJSON file containing shape data for zipcodes in King County & surrounding areas

zipcode_choropleth.html 
# Choropleth map highlighting average house prices by zipcode area

zipcodes-map.pdf
# An annotated map showing zip codes within the King County area

```

## Business Case and Brief

A property development company in Washington State wants to better understand the factors that influence the sale price of a property.

They are keen to use statistical modelling techniques to assist their decision making processes and better inform the planning, design and marketing of new build and / or renovated properties within the King County area.

Whilst we recognise that certain influencing factors are beyond the control of the developers, it is useful to understand their effect on the data.


## Approach

As outlined in the [Jupyter Notebook](index.ipynb) included in this repository, the approach constituted two main parts:

1. Initial **Exploratory Data Analysis** to review and validate the data fields available in the `kc_house_data.csv` dataset and understand each feature and their relationships both with each other and with the target variable, `price`.  The notebook contains several visualisations that are used in the [non-technical presentation](presentation.pdf) but also a choropleth map of average house price by zipcode.  Unfortunately the map does not appear inline within the notebook but in a [separate file](zipcode_choropleth.html).

![Average House Prices in King County 2014-15 by Zip Code](house-price-choropleth.png)

![Number of House Sales in King County 2014-15 by Zip Code](number-of-house-sales-by-zipcode.png)

2. The creation, refinement through iteration, validation and evaluation of a **Multivariate Linear Regression Model** including the use of stepwise feature selection, that highlights the influencing features and creates a prediction model for house prices in King County.


## Conclusions

The [Jupyter Notebook](index.ipynb#linear-regression) contains the details of each iteration of the linear regression model.  It was possible to create a [multivariate linear regression model](index.ipynb#model-v10) that, at first glance, produced a good predictive model with an R-Squared value of **0.843**.  However, on closer inspection, p-values for certain predictors are above 0.05 and therefore are not within acceptable bounds and the Jarque-Bera test score is too high suggesting that the distribution of residuals is not normal thereby not meeting one of the assumptions of linear regression.

After using [stepwise feature selection](index.ipynb#model-v11) and a more [manual approach](index.ipynb#model-v12) to refine the model further a satisfactory model was achieved with a R-Squared value of **0.559** but that had all predictors with p-values less than 0.05 and has a JB test score of **5.853**.

This final model was evaluated using both [train-test split](index.ipynb#model-evaluation-train-test-split) and [cross validation](index.ipynb#model-evaluation-cross-validation) with acceptable results.

The model shows the following impact on house prices in King County.

House prices tend to increase with increases in:
* Living Space (but this fluctuates between zip codes)
* Location (Waterfront)
* View

House prices tend to decrease with increases in:
* Lot Space



## Requisite Python Libraries

The following python libraries have been used as part of this project:

* [Pandas](https://pandas.pydata.org/)
* [NumPy](https://numpy.org/)
* [Seaborn](https://seaborn.pydata.org/)
* [Matplotlib](https://matplotlib.org/)
* [datetime](https://docs.python.org/3/library/datetime.html)
* [Folium](https://python-visualization.github.io/folium/)
* [JSON](https://docs.python.org/3/library/json.html)
* [scikit-learn](https://scikit-learn.org/)
* [statsmodels](https://www.statsmodels.org/stable/index.html)
* [SciPy](https://www.scipy.org/)