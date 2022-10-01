# king_county_housing_project
## Descripttion
The study was conducted to assist in prediction of housing prices in King County based on the presence of a waterfront, season, grade, region and number of bedrooms.
## Overview
The study is tasked with predicting the prices of houses in King County. The objective is to determine when it is most lucrative to sell houses and which regions are the most expensive in King County. The stakeholders for this study are homeowners, landowners and real estate agencies. The study's investigation was accomplished by data collection from the available online housing data on King County, using descriptive statistics and visualizations. The study discovered that the most expensive regions are Bellevue, Mercer Island and Newcastle with a mean aggregate price of 807,907 US dollars and Spring is the most expensive season with a mean aggregate price of 552782 US dollars.
## Business Understanding
The role assumed is that of a data scientist tasked with coming up with a linear model to predict the house prices in King County to help the following stakeholders:
* homeowners
* real estate agencies
* land owners

The analysis is based upon the following questions:
1. What features have a big impact in the price of a house?
2. How can we improve the value of a house?
3. Do prices vary by season of the year?
4. Do prices vary by the zipcode region?
### Data Description

The study made use of housing data provided by King County. The columns in the data set are as listed below:

* *id* - Unique identified for a house
* *date* - Date house was sold
* *price* - Price is prediction target
* *bedrooms* - Number of Bedrooms/House
* *bathrooms* - Number of bathrooms/bedrooms
* *sqft_living* - Square footage of the home
* *sqft_lot* - Square footage of the lot
* *floors* - Total floors (levels) in house
* *waterfront* - House which has a view to a waterfront
* *view* - Has been viewed
* *condition* - How good the condition is ( Overall )
* *grade* - overall grade given to the housing unit, based on King County grading system
* *sqft_above* - Square footage of house apart from basement
* *sqft_basement* - Square footage of the basement
* *yr_built* - Built Year
* *yr_renovated* - Year when house was renovated
* *zipcode* - Zipcode
* *lat* - Latitude coordinate
* *long* - Longitude coordinate
* *sqft_living15* - Square footage of interior housing living space for the nearest 15 neighbors
* *sqft_lot15* - Square footage of the land lots of the nearest 15 neighbors
## Summary of Exploratory Data Analysis
### Question 1: What features have a big impact in the price of a house?
The study took the position that the feature with very high correlation coefficient with price has the biggest impact on the price of a house.
The most correlated with price was *sqft_living* with a correlation coefficient of 0.7019173021377559
### Question 2: How can we improve the value of a house?
### Bedrooms
![image](https://user-images.githubusercontent.com/78497452/193420719-a8fe5206-fc3b-4edd-8e9b-308e51a80770.png)
![image](https://user-images.githubusercontent.com/78497452/193420740-10ff1e4e-be39-48c8-aee5-4f92afd68647.png)
* From the infographic above, the price of a house ceases to increase when an increase in the number of bedrooms is not coupled with an increase in square footage of the house above the basement.
* The correlation is moderately positive, meaning that the price of houses increases with an increase in the number of bedrooms as sqft_above increase upto a certain point. When the sqft_above starts to become small with an increase in bedrooms (reduced space) then the price of the house does not increase with the increase in number of bedrooms.
### Grade
![image](https://user-images.githubusercontent.com/78497452/193420832-7b91d877-f3d6-4a01-ac00-9887e994fa91.png)
![image](https://user-images.githubusercontent.com/78497452/193420881-7513bc45-f608-4532-88c0-081ac891c7aa.png)
* An increase in **grade** implies an increase in **price**

* To get beyond the price median, a house needs to be at least grade 10.

* The higher the square footage, the higher the grade.

* Lesser square footage houses need at least grade 7 to go beyond the price median.
### Waterfront
![image](https://user-images.githubusercontent.com/78497452/193420933-7a358d35-a66b-4d83-85e1-f3ab47e0273b.png)
![image](https://user-images.githubusercontent.com/78497452/193420940-5b26a5da-50ee-49cc-8ee5-8439f0d3e22e.png)
* With a waterfront, a house is guaranteed to be priced above the median but still there are houses without waterfront that are above median.
### Season
![image](https://user-images.githubusercontent.com/78497452/193420962-0ab8d05d-4de4-48e0-873f-549e1995e8f5.png)
#### sales_season and mean Price in USD
* Spring:	     552782.763271
* Summer:      546719.464286
* Fall:	       531276.474881
* Winter:	     519613.645467
* The season with the highest average price is Spring, during the months of March, April and May with an average price of 552782.76 US dollars while the season when prices are the least is winter which is during the months of December, January and February with a mean of 519613.65 US dollars.
### Zipcode
![image](https://user-images.githubusercontent.com/78497452/193421129-5f821661-6262-4be5-a352-7b359135c07e.png)
* Generally, houses with *waterfront* have higher prices and in C and G they are quite high with C having houses with high *sqft_above*.
* Area C looks to be a lavish area, an increase in *sqft_above* is followed by an increase in *price* more than any other place, with the most expensive houses being located in Area C, which is Bellevue, Medina, Mercer Island and Newcastle.
## Conclusion
* Houses sold in Spring are more expensive than other seasons.
* The median price of homes in King County is 450000.0 dollars
* The mean price of homes in King County is 540297 dollars
* The five highest priced regions are *Zip_C*, *Zip_G*, *Zip_B*, *Zip_A* and *Zip_I* in that order.
* Increase the square footage of the living space in the house
* Increase the square footage of the house apart from the basement
* Increase the number of bedrooms but also ensuring that the square footage above is also increased
* An increase in *grade* implies an increase in *price*
* To get beyond the price median, a house needs to be at least grade 10.
* The higher the square footage, the higher the grade.
* Lesser square footage houses need at least grade 7 to go beyond the price median.
* With a waterfront, a house is guaranteed to be priced above the median but still there are houses without waterfront that are above median.
* Houses that were renovated have a slightly higher price than those that are not renovated.
## Recommendations
### For a land owner
* A land owner would want to own land near a waterfront because they attract houses with higher prices.
* Having a parcel of land close to a waterfront would imply that it the land owner would have a strong bargaining chip given that a real estate agency would sell a house built on that parcel of land for a high price.
* The best waterfront properties with a high value in price are found in *Zip_C* around Bellevue, Mercer Island and Newcastle.
### For a home owner
* A home owner that seeks to get a high sell-on value would renovate the house in order to increase the condition and grade of the house. This drives up the price of the house since houses with renovation and houses with good conditions have a high value in terms of price.
* A home owner that is seeking to buy a good home would go for a home with high square footage above ground and a house with around 6-8 bedrooms since beyond 8 bedrooms the price of a house tend to decrease. This might be as a result of an increase in the number of bedrooms that is not followed by an increase in the square footage above ground. This would not be desirable for a homeowner due to congestion of the space.
* If the home owner wants to live in the 'expensive' residences and live a luxurious lifestyle then the homeowner would consider areas around *zip C* that have a waterfront.
* If an individual wants to be a homeowner in King County, the individual is adviced to make the purchase in Winter when the prices are relatively lower than other seasons.
### For real estate agencies
* A real estate firm looking to get value for their money should focus in areas around *zip_C* with a waterfront property.
* A real estate firm could also look to focus on properties with high square footage in the living area.
* A real estate firm could also renovate old properties to a very high grade and condition and then sell them for a good price.
* The firm should invest in houses of around 6 - 8 bedrooms since beyond that then an increase in the number of bedrooms is not desirable if the space is not big enough.
* A real estate firm looking to make the most profit should seek to sell the house in Spring when the prices are relatively higher than other seasons.
