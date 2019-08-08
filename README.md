
# Project 2 Ames Housing Data

### Problem Statement

> My brother has always looked forward to retiring in the future with a career in house flipping. Personally, I do not believe that it is a sustainable option as there are many things to consider when house flipping. House flipping for the uninformed is a way to make \"quick cash\" through making fast renovations. However, there are many features of a house that impact its final sales price. Using the Ames, Iowa housing data, I will see if there is any one neighborhood or house type that my brother can target to efficiently make a great return on investment.

---

### Datasets

The data set utilized were:

- [Train Data](./datasets/train.csv)
- [Test Data](./datasets/test.csv)

### Data Dictionary

- [Data Description](http://jse.amstat.org/v19n3/decock/DataDocumentation.txt)


---

### Executive Summary

The data is packed with 80 features of varying types. In order to pick the best features to include in my model, I first had to clean the data. This began with figuring out which columns had null values and deciding what to do with the nulls. To handle the null values, I imputed 'None' for object types and 0 for float or integer data types. After cleaning the data came visualizing the relationship between the different variables and sales price. After choosing the features for my model, I created 3 different models, linear regression, ridge and LASSO. For simplicity, I went with linear regression. 

Unforunately for Iowa, it was also heavily impacted by the 2008 housing market crash. This can be seen by the 48% drop in housing sales from 2009 to 2010 as well as a 4.5% drop in sales prices for the same time frame. As of 2019, Ames, Iowa ranked in the bottom 10 for least positive housing market outlooks [(source)](https://finance.yahoo.com/news/outlook-u-housing-market-hits-153300543.html). However, even with this bleak predicted outlook, there still stands a chance for house flipping and home renovations. THe current housing market is in dire need to new homes to accommodate for the increasing population [(source)](https://www.amestrib.com/news/building-ames-where-housing-market-stands-today).

---

### Conclusion and Next Steps 

Based on the analysis in part 2 of the EDA, it can be noted that while certain neighborhoods have benefits, they also come with their own negatives. For cheaper neighborhoods, while their remodeling rate was much higher than those of expensive ones, there is also the risk of being unable to gain a large ROI as all the other homes in the area are priced lower. With the expensive neighborhood, you run the risk of not being able to remodel enough to get a greater ROI. Also, as home prices in that area are more expensive, the price tag might make it harder to sell as quickly as possible. 

 Given all of this information, it will be useful to look into each neighborhood and change specific qualities of homes to see its predicted price. The model will be useful for being able to estimate house prices from a one unit change in certain features. It can estimate the ROI and isolate which houses have the most potential for remodeling. 
 
While the model incorporates many features, the data is still lacking in certain aspects. It would have been incredibly useful to have macroeconomic details. There is no information about the housing market crisis incorporated into this data set. Also, this model can only be utilized in terms of Ames. As quality is subjective, it can only work for the Ames home market. It would also be beneficial to have information on how remodeling effected home sale prices. The value of the house pre and post remodeling would be beneficial to see the magnitude of changing one feature over another.

---


