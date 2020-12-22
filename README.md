# Module 2 Final Project - Property Development in King County, Washington


## Overview
```
index.ipynb             # Jupyter notebook containing code for data discovery, EDA and the multivariate linear regression model
presentation.pdf        # A non-technical presentation of the project findings
kc_house_data.csv       # Raw dataset of house prices between 2014-15 for King County
zipcode_areas_king_county.geojson  # GeoJSON file containing shape data for zipcodes in King County & surrounding areas
zipcode_choropleth.html # Choropleth map highlighting average house prices by zipcode area
zipcodes-map.pdf

```

## The Business Case and Brief

A property development company in Washington State wants to better understand the factors that influence the sale price of a property.

They are keen to use statistical modelling techniques to assist their decision making processes and better inform the planning, design and marketing of new build and / or renovated properties within the King County area.

Whilst we recognise that certain influencing factors are beyond the control of the developers, it is useful to understand their effect on the data.


## Our Approach

As outlined in the [Jupyter Notebook](index.pynb) included in this repository, our approach constituted two main parts:

1. Initial **Exploratory Data Analysis** to review and validate the data fields available in the `kc_house_data.csv` dataset and understand each feature and their relationships both with each other and with the target variable, `price`.

2. The creation, refinement through iteration, validation and evaluation of a **Multivariate Linear Regression Model** including the use of stepwise feature selection, that highlights the influencing features and creates a prediction model for house prices in King County.


## Requisite Python Libraries

The following python libraries have been used as part of this project:

* Pandas
* NumPy
* Seaborn
* [Matplotlib](https://matplotlib.org/)
* [datetime](https://docs.python.org/3/library/datetime.html)
* [Folium](https://python-visualization.github.io/folium/)
* [JSON](https://docs.python.org/3/library/json.html)
* [scikit-learn](https://scikit-learn.org/)