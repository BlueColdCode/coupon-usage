# Coupon Usage Analysis

In this exercise, we apply the CRoss Industry Standard Process for Data Mining (CRISP-DM) process model to
prepare datasets and provide initial assessment of the information.

The provided dataset collected coupon usage information along with customers' background with regard to
family, education, gender, income, habits, as well as the situations where the coupons were applied, such
as weather, locations etc.

Because of our interests in coupon acceptance, the data processing becomes much simpler. In order to
extract prominent features that motivate people to use coupons, I wanted to separate the dataset based 
on coupon accepted or not, then do a conditional distribution of individual features using normalized 
histogram (KDE) by placing the conditional probabilities side-by-side as shown in the code, and arrived
at some interesting observations. The prominent features that decide coupon acceptance include:

 - Age: 21-30
 - Bar visits: more than once/month
 - Food carry-away: more than once/month
 - Coffee house visits: more than once/month
 - Type of coupon: 'Carry-out and Take-away', 'Restaurant(<20)'
 - Destination: 'No urgent place'
 - Education: high-school or non-degree college
 - Expiration: more than 1 day
 - Gender: Male
 - No children
 - Income: less than $50k or more than $100k
 - Marital status: single
 - Occupation: student
 - Passenger: friends
 - Temperature: hot (89-F)
 - Time: working-hours
 - Distance: short (<25 min)
 - Weather: sunny

We can combine the above factors in various ways to postulate that active people in
 working/studying hours in warm and good weather are more likely to use coupons.
