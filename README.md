[The link to the notebook](https://github.com/vilyapilya/used_cars/blob/main/prompt_II.ipynb) 

# Used Car Price Prediction

## Project Overview

This project analyzes a used car dataset to identify the factors that influence vehicle prices and give some recommendations to a car dealer on fine tuning their inventory. 

The analysis includes:
- Data cleaning and handling missing values. The data contained a lot of missing and low-quality values which where handled by performing different statistical inference methods. 
- Exploratory data analysis (EDA) to understand price distributions and relationships between features
- Feature engineering to improve model performance
- Machine learning modeling using regression techniques
- Model evaluation using MAE, MSE, and R² score

## Summary of Findings

The analysis showed that the most important features affecting car prices were related to vehicle age. According to permutation importance, **year**, **milage** and **manufacturer** had the strongest impact on price predictions.

Exploratory analysis revealed that:
- Newer vehicles generally have higher prices compared to older vehicles (apart from the retro models older than 80s - 90s).
- Mileage (odometer) negatively affects vehicle price, as vehicles with higher mileage tend to have lower prices.
- Different manufacturers have distinct price distributions, with luxury brands showing higher median prices. However, among the most common brands RAM and GMC have higher price distribution.
- Condition and titile status have either low or 0 impact on the price. 


The final regression model achieved:
- **pipe.score** 0.74  
- **Mean Absolute Error (MAE):** approximately $6,000  

This means the model explains about 74% of the variation in vehicle prices and makes predictions with an average error of around $6,000.

## Recommendation for the car dealers:
#%% md
### Next steps and recommendations:
1) Focus on the cars that are no older than 2010 if you're targeting mass-market brends.
2) RAM and GMC, Audi sustain the prices better than other makes.
3) If buying a Chrysler car, then consider that it most likely will not be sold for more than approximately 31,000 And 75% of them are sold for lower than 15,000. When the median price is less than 10,000. Buy Hyundai, Nissan and Honda with caution as well, 75% of them are sold for less than 20,000.
4) The paint color did not participate in the importance scaling, but the analyses has shown that white and black cars tend to be sold higher than other colors. The third place takes the orange color. And green cars have the lowest price distribution.


