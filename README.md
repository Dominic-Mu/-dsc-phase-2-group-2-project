# King County House Sales Prediction Project

**Authors**: [Dominic Muli](mailto:dominic.muli@student.moringaschool.com), [Allan Ngeiywa](mailto:allan.ngeiywa@student.moringaschool.com), [Celestine Imelda](mailto:celestine.imelda@student.moringaschool.com), and [Kevin Kagia](mailto:kevin.kagia@student.moringaschool.com)

## Project Overview

<img src="./images/kingcountylogo_mlk.webp" alt="KingCounty" height="100">

[King County](https://kingcounty.gov/en) situated in the U.S. state of Washington boasts a vibrant real estate market. This project conducts a comprehensive exploration of King County's housing landscape, aiming to unravel the factors that influence property prices.

## Business Problem
<img src="./images/vecteezy_debt-vector-icon_18897310.jpg" alt="Housing" height="100">
Home buyers in King County need advice on factors influencing housing prices.

## Objectives
We will use data analytics and predictive modeling techniques to provide homeowners, buyers, and investors with valuable insights for making informed decisions in this thriving real estate market.

Specifically, we will:

* Analyze the relationship between house prices and factors such as square footage, number of bedrooms and bathrooms, location, waterfront and view, condition and renovation status.
* Identify the most important factors that affect house prices.
* Develop predictive models that can be used to estimate the future price of a house.
* Share our findings through presentation.
We believe that this project will provide valuable insights into the King County housing market and help people make informed decisions about their real estate investments.

## Metric of Success
The project will be considered successful if:
* We accurately make predictions about housing prices and explain factors influencing house prices.
* Our models generate new useful data
* We generate useful recommendations to home buyers to make informed decisions

## Understanding Data
The data for this project will be obtained from the King County property appraiser website.
The dataset has the following variables:
* `id` - Unique identifier for a house
* `date` - Date house was sold
* `price` - Sale price (prediction target)
* `bedrooms` - Number of bedrooms
* `bathrooms` - Number of bathrooms
* `sqft_living` - Square footage of living space in the home
* `sqft_lot` - Square footage of the lot
* `floors` - Number of floors (levels) in house
* `waterfront` - Whether the house is on a waterfront
  * Includes Duwamish, Elliott Bay, Puget Sound, Lake Union, Ship Canal, Lake Washington, Lake Sammamish, other lake, and river/slough waterfronts
* `view` - Quality of view from house
  * Includes views of Mt. Rainier, Olympics, Cascades, Territorial, Seattle Skyline, Puget Sound, Lake Washington, Lake Sammamish, small lake / river / creek, and other
* `condition` - How good the overall condition of the house is. Related to maintenance of house.
  * See the [King County Assessor Website](https://info.kingcounty.gov/assessor/esales/Glossary.aspx?type=r) for further explanation of each condition code
* `grade` - Overall grade of the house. Related to the construction and design of the house.
  * See the [King County Assessor Website](https://info.kingcounty.gov/assessor/esales/Glossary.aspx?type=r) for further explanation of each building grade code
* `sqft_above` - Square footage of house apart from basement
* `sqft_basement` - Square footage of the basement
* `yr_built` - Year when house was built
* `yr_renovated` - Year when house was renovated
* `zipcode` - ZIP Code used by the United States Postal Service
* `lat` - Latitude coordinate
* `long` - Longitude coordinate
* `sqft_living15` - The square footage of interior housing living space for the nearest 15 neighbors
* `sqft_lot15` - The square footage of the land lots of the nearest 15 neighbors


## Methods
We will use a variety of data analytics and predictive modeling techniques to analyze the data and develop our models. These techniques will include:

* Exploratory data analysis
* Feature selection
* Model training and evaluation
* Model deployment

## Conclusions
* The overall model fit is reasonable, with an R-squared value of approximately 0.676. This means that around 67.6% of the variability in house prices can be explained by the combination of independent variables included in the model. 
* Several independent variables show statistically significant relationships with house prices. These include:

 * Bedrooms: The number of bedrooms has a negative effect on house prices.
 * Bathrooms: More bathrooms tend to increase house prices.
 * Square Footage: An increase in square footage positively impacts house prices.
 * Waterfront Property: Having a waterfront location significantly increases house prices.
 * Condition: Better property condition is associated with higher house prices.
 * Grade: Higher property grades positively affect house prices.
 * Year Built: Older homes tend to have lower prices, while newer homes have higher prices.
 * Year Renovated: Renovations positively impact house prices.
 * Location (Zipcode, Latitude, Longitude): These location-related variables significantly influence house prices.
### Recommendations
* Property Improvement: Consider investing in property improvements, such as renovating or upgrading certain features, to potentially increase the property's value.
* Location Matters: The location of the property, as indicated by variables like zipcode, latitude, and longitude, plays a significant role in house prices.
* Bedrooms and Bathrooms: The number of bedrooms and bathrooms can affect prices. Sellers should highlight these features, and buyers should consider their needs.
* Square Footage: Increasing square footage can positively impact property value. Sellers may benefit from maximizing usable living space.
* Waterfront Properties: Waterfront properties command higher prices. Buyers interested in such properties should expect premium pricing.
* Age of the Property: Older properties tend to have lower prices, so buyers should consider the trade-offs between historic charm and modern amenities.
* Condition and Grade: Sellers should focus on property condition and grade to potentially increase market appeal and pricing.

In summary, this regression analysis provides insights into the factors influencing house prices in the dataset. However, it's essential to consider these results as a tool to inform decisions, rather than a definitive predictor. Real estate prices can be influenced by various external factors, and local market conditions may vary. Continual analysis and market awareness are key to making informed decisions in the real estate market.

## For More Information

See the full analysis in the [Jupyter Notebook](./house_prices_prediction.ipynb) or review this [presentation](./house_prices_prediction.pdf).

For additional info, contact [Dominic Muli](mailto:dominic.muli@student.moringaschool.com), [Allan Ngeiywa](mailto:allan.ngeiywa@student.moringaschool.com), [Celestine Imelda](mailto:celestine.imelda@student.moringaschool.com), and [Kevin Kagia](mailto:kevin.kagia@student.moringaschool.com)

## Repository Structure
```
├── data
├── images
├── house_prices_prediction.ipynb
├── house_prices_prediction.pdf
└── README.md
```