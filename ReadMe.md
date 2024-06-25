Page Visits Funnel Project
This project analyzes the journey of users through an e-commerce site using data from visits, carts, checkouts, and purchases.

Project Overview

- The goal of this project is to understand the drop-off rates at different stages of the shopping funnel:

1 - Visitors who visit the page
2 - Visitors who add items to their cart
3 - Visitors who proceed to checkout
4 - Visitors who complete a purchase

Files

visits.csv: Contains information about user visits to the page.
cart.csv: Contains information about users adding items to their cart.
checkout.csv: Contains information about users proceeding to checkout.
purchase.csv: Contains information about users completing a purchase.

Steps

1 - Reading the Data:
We read the CSV files into pandas DataFrames and parse dates as datetime objects for better analysis.

2 - Merging DataFrames:
We perform left joins to combine data from different stages:

visits with cart
cart with checkout
Combining all data into all_data

3 - Analyzing Drop-offs:
We calculate the number of users at each stage and the percentage drop-off at each step:

Total visits
Visits with no cart addition
Checkouts with no purchase

4 - Percentage Outputs:
We print the percentages of users who drop off at each stage.

5 - Time to Purchase:
We calculate the average time it takes for a user to make a purchase from their initial visit.

Summary
This project helps in understanding where users drop off in the e-commerce funnel, providing insights into user behavior and areas that need improvement to increase conversion rates.
