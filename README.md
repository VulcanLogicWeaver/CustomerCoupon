# CustomerCoupon
Practical Application Assignment 1
This assignment is to analyze those who accepted and rejected coupons.

The data is provide in a file labeled "coupons" as a csv file, placed in the 'data' directory [https://github.com/VulcanLogicWeaver/CustomerCoupon/blob/main/data/coupons.csv] The code to analyze all the different scenarios is in the jupyter notebook "Customer Coupon Project.ipynb" in the main directory [https://github.com/VulcanLogicWeaver/CustomerCoupon/blob/main/prompt.ipynb]

Data overview:
- The data set has good about of data, about 12684 rows.
- The column labeled 'car' seem to have the most empty or null values, and does not seem to have any influence on the analysis. Hence decided to not use this column as part of data cleanup.
- Decided to convert the age column from string to integer, which can them be used for arithmetic operations

Data Analysis:
- Overall about 56% have chosen to accept coupons
- A bar plot was generated to visualize the various type of coupon category. And from the chart it seem Male and Female have similar proportions of coupons
- Further analysis was all focused on Bar coupons. About 40% of Bar coupons were accepted. Multiple sub categories were used to further analyze the data:
--  Frequent Bar visitors [more than 3 times a week] vs. Less frequent Bar visitors: it seems like frequent bar visitors are 2 times more likely to accept Bar coupon than less frequent visitors
--  Frequent Bar visitors [more than once a week and above age 25]: similar to above, frequent bar visitors have twice as likely accepted coupons
--  Frequent Bar visitors [more than once a week with adult passenger and not farming, fishing, or forestry industry: similar results as above: frequent visitors as twice as likely to accept coupon
--  Frequent Bar visitors with multiple criteria has a similar pattern

Overall, it seems that frequent visitors are twice or more likely to accept coupons than less frequent visitor As part of independent investigation, built a (n x n) dataframe to visualize the coupon acceptance over various income ranges and between Male and Female groups. There are certainly some interesting patterns, the middle income range ($37,500 - $49,999) Female category seem to have accepted the most coupons and lowest income range (less than $12,500) Female category seem have accepted the least amount of coupons.
Similar analysis can be performed with other data columns, drivers proximity to the establishment, direction of the driver, etc.
