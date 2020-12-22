# Column Names and descriptions for Kings County Data Set

* **id** : a unique identifier for a property
* **date** : date property was sold (note: uses US date formatting)
* **price** : sale price (target variable)
* **bedrooms** : number of bedrooms
* **bathrooms** : number of bathrooms (note: includes half and quarter bathrooms, e.g. a "half bathroom" would be a toilet & sink) [view more detail](https://www.kaggle.com/harlfoxem/housesalesprediction/discussion/24804)
* **sqft_living** : square footage of the living space
* **sqft_lot** : square footage of the plot of the property
* **floors** : number of floors (levels) in the property (note that there are half floors)
* **waterfront** : dummy variable indicating that property has a view to a waterfront (boolean)
* **view** : a rating, between 0 and 4, describing the view of the property
* **condition** : a rating, between 1 and 5, describing the overall condition of the property, [view full detail](https://info.kingcounty.gov/assessor/esales/Glossary.aspx?type=r#building%20condition)
    * 1 - Poor
    * 2 - Fair
    * 3 - Average
    * 4 - Good
    * 5 - Very Good
* **grade** : overall grade given to the property unit representing the construction quality of improvements, [view full detail](https://info.kingcounty.gov/assessor/esales/Glossary.aspx?type=r#building%20grade)
    * 1-3 - Falls short of minimum building standards
    * 4 - Generally older, low quality construction, does not meet code
    * 5 - Low construction costs and workmanship, small, simple design.
    * 6 - Lowest grade currently meeting building code, low quality materials and simple designs.
    * 7 - Average grade of construction and design.
    * 8 - Just above average in construction and design. Usually better materials in both the exterior and interior finish work.
    * 9 - Better architectural design with extra interior and exterior design and quality.
    * 10 - Homes of this quality generally have high quality features. Finish work is better and more design quality is seen.
    * 11 - Custom design and higher quality finish work.
    * 12 - Custom design and excellent builders, all materials are of the highest quality.
    * 13 - Generally custom designed and built, large amount of highest quality cabinet work, wood trim, marble, entry ways etc.
* **sqft_above** : square footage of property above and including ground floor
* **sqft_basement** : square footage of the property below ground floor (i.e. the basement)
* **yr_built** : year the property was built
* **yr_renovated** : year the house was renovated
* **zipcode** : zip code of the property
* **lat** : latitude coordinate of the property
* **long** : longitude coordinate of the property
* **sqft_living15** : the average square footage of interior housing living space for the nearest 15 neighbours
* **sqft_lot15** : the average square footage of the land plots of the nearest 15 neighbours