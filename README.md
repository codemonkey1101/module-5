# Module 5: Using what was learned in the first 4 modules

### Diagnosing Usage of Bar Coupons by a Driver Who has received the coupon via their Phone

## Observations:

Only 785 drivers used the bar coupons out of 1906 who received them.
# Out of the 785 drivers the following propogations were examined
Top 4 Income: 
- $25000 - $37499     136
- $100000 or More     134
- $12500 - $24999     114
- $50000 - $62499     101

![image](images/income_accepted_bar_coupons.png)


Top 4 Occupation:
- Student                       114
- Unemployed                    87
- Computer & Mathematical       79
- Sales & Related               78

It was difficult for me to accept the data regarding occupation in relation to income being that there were students and unemployed drivers shown as making $100,000 which didn't make any sense.  I could have filtered out those data points and used some of the student data but being that most students are potentially under the age of 21 I would think a retail business like a bar, which has age restrictions, would want to remove that demographic any way for legal reasons.  Furthermore, with regards to age people >=21 and < 36 did the bulk of the accepting anyway so not being able to use the "Student" demographic was really a non-issue.

There seemed to be a strong acceptant when looking at drivers in specific age groups that were non-parents vs parents

Parental status (has_children)
- Parents       241
- non parents   544 

![image](images/bar-coupon-all_ages-parental_status.png)


With that observation, age was another data point where driver's between the ages of 21 and 35 seemed to accept coupons more often then not.  Especially when they did not have parental responsibilities

Total bar coupons accepted when associated with a driver's age

Top 4 Age groups:
- 21-25    200
- 26-30    179
- 31-35    121

Another good target scenario that I observed was when I associated the driver's "destination" and "outside temperature".  It was noted that as temperatures went up and the driver had no real urgency to go anywhere, the bar seemed to be the place of choice.  Similarly it was seen that when the temperature was not too hot and not too cold (55 deg), regardless of urgency, drivers tended to accept the bar coupon more often then not.  I was able to observe this from the folling bar chart.

![image](images/temp_and_travel_waccepted_bar_coupons.png)


## Hypothesis

After seeing the effect of temperature I decided to compare that with age.  Here it was observed the driver's between the ages of 21 and 30 accepted bar coupons the most over any other relation.  However, this same behavior was exibited during moderate temperatures as shown in the following diagram.

![image](images/bar-coupon-all_ages-by_temp.png)

This would suggest a possible correlation between the two.  So, when the temperature is 55 degrees similar behavior could be expected when dealing with specific age groups when drivers were not parents.  Unfortunately, given the nature of the dataset I was not able to prove any correlation actually existed.


#### Independent Investigation

### Using the cheap restaurant ($ < 20) coupon I attempted to determin how passangers and drivers influence each other with regards to accepting this type of coupon.

## Observations:

The total number of accepted coupons of this type was 1878.

The examined propoated data for restaurant<20 coupons was as follows:

Age:
- 21-25    403
- 26-30    388
- 31-35    294
- > 50     243
- 36-40    182
- 41-45    174
- 46-50    107
- < 21      87

Passanger:
- Alone        1365
- Friend(s)     789
- Kid(s)        249
- Partner       243

Gender:
- Female    940
- Male      938

Parents (1) vs Non-parents (0):
- 0    1128  ( 60.06% )
- 1     750  ( 39.94% )

When comparing parents vs non-parents, the parents accepted these types of coupons ~40% of the time vs ~60% by non-parents (as shown in the following bar chart).

![image](images/accepted_rest_less20_coupons_for_parents_and_non_parents_by_age.png)

For that reason I focused mainly on the non-parents in this effort.

It was observed that younger men, between the age of 21 and 30, tended to accept the coupons far more often then their older counter parts, regardless if they were alone or with an adult passanger.  However, women within that same age group perferred to eat out with an adult companion (or passanger that was not a child).

![image](images/accepted_rest_less20_coupons_for_pass_w_non_parents_by_age.png)

Furthermore, it was observed that as both men and women got older they accepted these coupons far less.  This observation was very similar to the one done with bar coupons and again would suggest a correlation between the two.
