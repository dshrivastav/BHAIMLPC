# BHAIMLPC 5.1
Berkeley AI ML 
# Assignment 5.1: Will the Customer Accept the Coupon?
This program, seeks to answer the question, “Will a customer accept the coupon?” The goal of this project is to use visualizations and probability distributions to distinguish between customers who accepted a driving coupon versus those who did not. 
# Data
This data is from the UCI Machine Learning Repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios, including the destination, current time, weather, and passenger, and then asks people whether they will accept the coupon if they are the driver. There are three possible answers people can choose from:

“Right away”
“Later, before the coupon expires”
“No, I do not want the coupon”
The first two responses are labeled as “Y = 1,” and the third is labeled as “Y = 0.” There are five different types of coupons: Less expensive restaurants (under $20), coffee houses, carryout and takeaway, bars, and more expensive restaurants ($20–$50).

# Data exploration and preparation
The data had some missing values, and especially the car column is missing a large number of values, hence not useful for any analysis.
Cleaned the data by dropping the rows with null values except Car. If car column is included for dropping the values then pretty much all rows would get dropped, hence skipped it.
Converted the age and income columns to numneric values so arithmentic operators could be applied to them.
The jupyter notebook depicts visualizations for the Bar and the CarryAway coupon categories.  

# Findings
Based on the analyses and observations, we can hypothesize the following about drivers who accepted bar coupons:

## 1. Frequency of Bar Visits
Drivers who frequent bars more than once a month are more likely to accept bar coupons compared to those who visit bars less often. This indicates that the acceptance rate correlates with a preexisting interest or habit of visiting bars.

## 2. Demographic Factors
Age: Younger drivers (under 30) are more inclined to accept bar coupons, likely due to lifestyle preferences and social habits.
Marital Status: Drivers who are not widowed, possibly indicating a more active social lifestyle, show a higher acceptance rate.
Income: Drivers with lower incomes (<$50K) and who visit cheap restaurants more frequently might be more price-sensitive, making them more receptive to discounts like coupons.

## 3. Passenger Dynamics
Drivers with passengers who are not kids tend to accept bar coupons more often. This could suggest that passengers like friends or partners influence the decision to go to a bar, especially when a discount is available.

## 4. Occupation
Drivers with occupations other than farming, fishing, and forestry are more likely to accept bar coupons. This could relate to geographic or cultural factors where bar visits might be less common among those in certain professions or rural settings.

## 5. Lifestyle Influence
Drivers who exhibit higher frequencies of leisure activities (like eating at cheap restaurants or visiting bars) tend to accept coupons at a higher rate. This reflects a predisposition toward cost-saving behaviors in their social habits.

# Conclusions
## 1. Drivers who accepted Bar coupons 
Drivers who accepted bar coupons are generally younger, socially active, price-conscious, and often accompanied by friends or partners. They are more likely to engage in leisure activities, live in urban or suburban settings, and demonstrate higher acceptance of promotions aligned with their lifestyle preferences.

## 2. CDrivers who accepted CarryAway coupons
Based on a similar analysis for the Carry Away coupons, it is clear that this type of coupon had a pretty high acceptance rate of 73.77%. Overall, factors like kids and age did not impact the carry away coupon acceptance rate. However, it appears that people from urban and sub-urban background are more likely to accept carry out and take away coupons than those who are in farming, fishing and rural background.

## 3. Recommendations
Given that the driver behaviors and demographics correlate with higher coupon acceptance rates, following is recommended for marketing purposes.
1. Bar coupons should be targeted for marketing to younger drivers, who are socially active, price conscious
2. Both Bar and CarryAway coupons be targeted for marketing for drivers in urban and sub-urban setting.

