# Mod11_AIMLPA2
Used Car Price Prediction – Report
Project Overview

We analyzed a dataset of 426K used cars (subset of a larger 3M record dataset from Kaggle) to understand the factors influencing resale prices in the U.S. car market.

The problem was framed as a regression task, applying machine learning models including Linear Regression, Decision Trees, and Random Forests. Their performances were compared to identify the most suitable technique for predicting used car prices.

This work follows the CRISP-DM process, from data understanding and preparation to modeling and deployment, ensuring insights are both data-driven and practical for dealership operations.

Key Data Insights

Car Age

Older cars are generally cheaper than newer ones.

Most cars in the dataset are less than 15 years old.

Manufacturers

Ford and Chevrolet dominate the dataset.

Premium manufacturers like Volvo and Toyota show stronger resale value.

Fuel Type

Vast majority run on gas.

Diesel vehicles, although fewer, tend to retain higher resale prices.

Condition & Title

Nearly every car is listed with a “clean” title, limiting predictive power of this variable.

Reported condition (good/excellent) has only mild variation.

Mileage (Odometer)

65% of vehicles have mileage < 50K miles.

Strong negative correlation: higher mileage → lower resale price.

Modeling Results

Linear Regression gave a baseline but struggled with skewed distributions.

Decision Trees captured non-linearities but overfit in some cases.

Random Forests performed best overall, balancing bias/variance and handling outliers better.

Recommendation: Use Random Forests (or Gradient Boosted Trees for deployment) for production price prediction.

Key Findings on Price Drivers

Manufacturer & Vehicle Type are the strongest determinants of price.

Positive impact: Volvo, Toyota, Pickup trucks, Diesel fuel, Manual transmission.

Negative impact: RAM, Datsun, Harley-Davidson, Offroad vehicles, Hybrids (in this dataset context).

Feature interactions matter:

Example: A Volvo pickup, diesel, manual transmission → higher resale value.

Example: A Datsun offroad hybrid → lower resale value.

Mileage & Age remain consistent downward drivers of value, but less influential than manufacturer/type in this dataset.
