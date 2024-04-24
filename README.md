# assignment_11.1
 Practical Application Assignment 11.1

This repo contains the Jupiter Notebook for Assignment 1-1 which can be found here: 
https://github.com/rcolcord/assignment_11.1/blob/main/prompt_II.ipynb

Summary of Methods

Multiple linear regression-derived models were developed to determine the relative impact of each used car feature (the feature coefficient) on the price. The following models were developed:
- Basic linear regression
- Sequential feature selection with linear regression
- Backward feature selection with linear regression
- Ridge regression
- Lasso regression


Key Assumptions and Decisions
- A local used car dealership doesn't care about region/state as they can't change their location
- The model of the car was removed as it contained too many variables and would bog down or over-complicate the model


Key Findings

The linear regression model performed the best, as determined by cross-validation. The Ridge and Lasso models performed comparable, so these models were aggregated to determine the average coefficient for each feature across the three models. Examining the coefficients for each feature, we can observe the following findings:
- The most important factor in determining the price of a used car is the manufacturer. This goes in both directions - positive and negative.
  - The manufacturers with the largest positive impact on price were Ferrari, Tesla, Aston-Martin, Porsche, Datsun, and Alfo-Romero. The first four had the most outsized effect.
  - The manufacturers with the largest negative impact on price were Fiat, Saturn, Mercury, Chrysler, Subaru, Mini, Nissan, Kia, Mazda, Hyundai
- Diesel and electric fuel types had a large positive impact on price.
  - Gas and hybrid vehicles had moderate negative impacts on price
- The number of cylinders had a moderately large impact on price
  - 8 and above cyliners had a large impact on price, while anything less than 8 had relatively moderate negative impacts
- The condition of the car and the model year both had moderately large positive effects on price, as expected. However, the impact of the car condition was greater than the impact of model year.
- The type of car had a moderate impact on price in both directions
  - Convertibles, coupes, trucks, offroad, and vans had positive impacts whereas sedans, wagons, SUVs, hatchbacks and minivans had negative impacts. Pickups had negligible impact.
- The size of vehicles had a small impact on price. Full-size and mid-size vehicles had small positive impact, while compacts and sub-compacts had small negative impact
- Paint color had a mostly small impact in both directions, with the exception of the color orange, which had a moderately large positive impact on price

![top10neg](https://github.com/rcolcord/assignment_11.1/assets/160987886/7b4abb64-0ce3-4e94-ad30-519d3de21e92)
![top10pos](https://github.com/rcolcord/assignment_11.1/assets/160987886/d4fb13c8-8065-4958-b44e-01e23471418a)


Recommendations
If the goal of the dealership is to maximize selling prices and increase revenue, we recommend focusing on the following features when selecting inventory:
- High-end manufacturing brands, specifically Ferrari, Tesla, Aston-Martin, and Porsche.
- Specialized fuel types - specifically diesel and electric - over gas and hybrid
- Prioritize higher cylinder counts
- Better condition cars and newer model years - favor condition over year
- Prioritize convertible, coupes, trucks, and offroad vehicles over sedans, wagons, SUVs, and hatchbacks.
- Orange and yellow cars. Avoid brown cars
