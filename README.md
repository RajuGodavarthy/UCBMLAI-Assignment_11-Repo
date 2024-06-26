# Used Car Price Prediction Project

## Overview

The goal of this project is to analyze the factors that influence the price of used cars. By leveraging statistical and machine learning techniques, we aim to identify key drivers of car prices and provide actionable recommendations to a used car dealership based on consumer preferences.

## Data

- **Source:** Data downloaded from Kaggle
- **Features:**
  - **id:** Numerical index
  - **region:** Region or city where the car is located
  - **price:** Price of the car (target variable)
  - **year:** Year the car was manufactured
  - **manufacturer:** Manufacturer of the car
  - **model:** Model of the car
  - **condition:** Condition of the car
  - **cylinders:** Number of cylinders
  - **fuel:** Fuel type used by the car
  - **odometer:** Mileage recorded on the car's odometer
  - **title_status:** Title status of the car
  - **transmission:** Type of transmission
  - **VIN:** Vehicle Identification Number
  - **drive:** Drive type (e.g., 4WD, RWD)
  - **size:** Size of the car
  - **type:** Type of the car (e.g., SUV, sedan)
  - **paint_color:** Color of the car
  - **state:** State where the car is located

## Deliverables

- Identify key drivers of used car prices and frame this as a data problem.
- Create a predictive model using statistical and machine learning techniques to analyze the dataset and determine which factors most significantly influence used car pricing.

## Findings

### Coefficients Analysis

Each coefficient from the Lasso regression model represents the estimated change in the predicted used car price (in dollars) for a one-unit increase in each respective feature, holding all other features constant:

- **region:** 34.308565
- **year:** 32.298957
- **manufacturer:** 29.723986
- **model:** 77.860309
- **fuel:** 7.195754
- **odometer:** 10.426611
- **title_status:** 71.873079
- **transmission:** 9.316824
- **state:** 5.413494
- **age:** 59.602569

### Interpretation

- **Model:** Each unit increase in the car model is associated with an increase of approximately $77.86 in the predicted price.
- **Title Status:** Each unit increase in title status (e.g., clean title) is associated with an increase of about $71.87 in the predicted price.
- **Age:** A newer car (lower age) has a significant positive impact on price.
- **Region and Manufacturer:** These factors also positively influence price but to a lesser extent compared to model and title status.
- **Fuel, Odometer, Transmission, State:** These features have relatively lower impacts on the used car price.

### Recommendations

Based on these findings:
- Emphasize the importance of the car model and title status in pricing strategies.
- Highlight the value of newer cars to potential buyers.
- Consider regional and manufacturer preferences but prioritize model and title status in pricing decisions.

## Conclusion

This analysis provides insights into what factors drive the price of used cars, helping the client—a used car dealership—to understand consumer preferences better. By focusing on these key drivers, the dealership can optimize pricing strategies and enhance customer satisfaction.

---

This README file summarizes the project's objectives, data sources, findings from the analysis of Lasso regression coefficients, and actionable recommendations for the client. It provides a clear and structured overview for stakeholders to understand the project's outcomes and implications effectively.
