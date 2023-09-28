Author: Abdul Ghouse
Version: 1.0
Date: 07/10/2023

Jupiter Note Book location:
https://github.com/aaghouse/aimlrepo/tree/main/AmazonML-coupon-analysis/Amazon_UCI_ML_coupon_accept_analysis.ipynb 

README File location:
https://github.com/aaghouse/aimlrepo/edit/main/AmazonML-coupon-analysis/README.md

Detailed Results File location:
https://github.com/aaghouse/aimlrepo/tree/main/AmazonML-coupon-analysis/Analysis-results.txt

---------------------------------------------------------------------------------------------------------------------------------------
---------------------------------------------------------------------------------------------------------------------------------------

## Will a Customer Accept the Coupon?
### Context
Imagine driving through town and a coupon is delivered to your cell phone for a restaraunt near where you are driving. Would you accept that coupon and take a short detour to the restaraunt? Would you accept the coupon but use it on a sunbsequent trip? Would you ignore the coupon entirely? What if the coupon was for a bar instead of a restaraunt? What about a coffee house? Would you accept a bar coupon with a minor passenger in the car? What about if it was just you and your partner in the car? Would weather impact the rate of acceptance? What about the time of day?

Obviously, proximity to the business is a factor on whether the coupon is delivered to the driver or not, but what are the factors that determine whether a driver accepts the coupon once it is delivered to them? How would you determine whether a driver is likely to accept a coupon?

Overview
The goal of this project is to use what you know about visualizations and probability distributions to distinguish between customers who accepted a driving coupon versus those that did not.

Data
This data comes to us from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios including the destination, current time, weather, passenger, etc., and then ask the person whether he will accept the coupon if he is the driver. Answers that the user will drive there ‘right away’ or ‘later before the coupon expires’ are labeled as ‘Y = 1’ and answers ‘no, I do not want the coupon’ are labeled as ‘Y = 0’. There are five different types of coupons -- less expensive restaurants (under $20), coffee houses, carry out & take away, bar, and more expensive restaurants ($20 - $50).

Deliverables
Your final product should be a brief report that highlights the differences between customers who did and did not accept the coupons. To explore the data you will utilize your knowledge of plotting, statistical summaries, and visualization using Python. You will publish your findings in a public facing github repository as your first portfolio piece.

---------------------------------------------------------------------------------------------------------------------------------------
---------------------------------------------------------------------------------------------------------------------------------------
Summary of findings: Hypothesis on Coupon acceptance based of the drivers who accepted the coupon
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
![histogram-of-accepted-coupons-by-coupon-category](https://github.com/aaghouse/aimlrepo/assets/90729963/a04b917b-8fb5-417c-9e50-d2f40aeac8e8)
![bar-gt1time-nkids-nwidowed-marital-status-accept-count](https://github.com/aaghouse/aimlrepo/assets/90729963/c61d5ab9-0152-401a-8afa-c366d3f65cf5)
Observation:
Single, married partner and unmarried partners visiting bar > 1 time seem to overwhelmingly accept coupons.
Timing of the coupon (peak-driving times) offer impacts acceptance rate greatly, best times are 6:00PM, 7:00AM and 10:00AM
It also appears single people, married/unmarried couple seem to visit bar more often and they are the ones who accept the coupon.
Coupons tend to be accepted closer (5 mins drive) locations much more often
then others (100% acceptance rate).Followed by 15 min drive destinations(51%
acceptance rate) and lastly followed by 25 min drive locations (9.6%).
People accept coupons with expiration of 1 day compared to 2hours. This
indicates they are like to choose their preferred time rather than rushed to use
the coupon.

People decline coupons if the copons are presented at the off-peak work hours
2pm or 10pm. (or) If the coupon is in the same direction as they are going to
their destination (indicating them reaching their destination is higher
priority, potentially these are gig workers lyft of Uber). Coupons get
declined also if they are more than 15 mins or 25Mins to their coupon destination.

![drivers_driving_opp_dir_accepting_coupon](https://github.com/aaghouse/aimlrepo/assets/90729963/9e12ab98-0a1f-4273-ac2d-dc6dd07ee695)
If we want to get more acceptance of the coupons potential groups of people
to target are single/married-partner/unmarried-partner groups driving.
People going to bars more than ones are also good targets. Favorable times to
get the coupons to be accepted are 6:00PM, 7AM and 10AM. ( peak driving hours)
It would also be favorable to give the coupons to drivers in the opposite
direction of their driving destination allowing them time to complete their
driving goals.
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
