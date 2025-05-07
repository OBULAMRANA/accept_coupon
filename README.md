Project: Module 5 Practical Application Example 1
===

# Author: Rana Obulam

Dataset information
---
Imagine driving through town and a coupon is delivered to your cell phone for a restaurant near where you are driving. Would you accept that coupon and take a short detour to the restaurant? Would you accept the coupon but use it on a subsequent trip? Would you ignore the coupon entirely? What if the coupon was for a bar instead of a restaurant? What about a coffee house? Would you accept a bar coupon with a minor passenger in the car? What about if it was just you and your partner in the car? Would weather impact the rate of acceptance? What about the time of day?

Obviously, proximity to the business is a factor on whether the coupon is delivered to the driver or not, but what are the factors that determine whether a driver accepts the coupon once it is delivered to them? How would you determine whether a driver is likely to accept a coupon?

**Overview**

The goal of this project is to use what you know about visualizations and probability distributions to distinguish between customers who accepted a driving coupon versus those that did not.

**Data**

This data comes to us from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios including the destination, current time, weather, passenger, etc., and then ask the person whether he will accept the coupon if he is the driver. Answers that the user will drive there ‘right away’ or ‘later before the coupon expires’ are labeled as ‘Y = 1’ and answers ‘no, I do not want the coupon’ are labeled as ‘Y = 0’.  There are five different types of coupons -- less expensive restaurants (under \$20), coffee houses, carry out & take away, bar, and more expensive restaurants (\$20 - $50).

Data Source: [https://github.com/OBULAMRANA/accept_coupon/blob/main/coupons.csv](https://github.com/OBULAMRANA/accept_coupon/blob/main/coupons.csv)

Python Code: [https://github.com/OBULAMRANA/accept_coupon/blob/main/accept_coupon.ipynb](https://github.com/OBULAMRANA/accept_coupon/blob/main/accept_coupon.ipynb)

Note: There are no errors in the code
Given dataset has total 12684 entries with 26 columns and null information contains 6 columnss(car,Bar,CoffeeHouse,CarryAway,RestaurantLessThan20,Restaurant20To50)

Data Understanding  and cleanup.**
---

1.car	12576

2.Bar	107

3.CoffeeHouse	217

4.CarryAway	151

5.RestaurantLessThan20	130

6.Restaurant20To50	189

Data Understanding  and manupulate the data.**
---
 1. passanger column values contains Kid(s) and Friend(s). This data got replaced with Kids and Friends respectively.
 2. Income column has 3 types of values below 50K. Those values($37500 - $49999, $12500 - $24999, $25000 - $37499) got replaced with below50k
 3. RestaurantLessThan20 column has 2 types of values greater than 4. Those values(4~8 , gt8) got replace with gt4/

 Types of Coupons accepted and rejected from the original dataset  
---
![image](https://github.com/user-attachments/assets/ec3700f9-d9d9-45d9-a20b-33bbb85f765c)

Different types of coupons original dataset  
---
 ![image](https://github.com/user-attachments/assets/c8ae0579-e3e4-4767-b677-1eacc86e354f)

Histogram 
---
![image](https://github.com/user-attachments/assets/ce3b9745-0d3f-4b7a-b693-9080f3b10ce0)

Coupons Accepted/Rejected
---
![image](https://github.com/user-attachments/assets/09ac1ef5-6651-4477-8fc5-0e01a25b0944)

Acceptance rate comparision (Under 25 and Above 25)
---
![image](https://github.com/user-attachments/assets/e048a629-cc20-437d-aead-7911bdb891af)

Acceptance rate comparision (no kids,other than farming,went more than once to bar)
---
![image](https://github.com/user-attachments/assets/34ee0e05-3f49-48db-89c1-a8c17ec3e034)

Acceptance rate comparision (under-30', 'no-kids-widow', 'bar more than 4 times -Income less than 50K)
---
![image](https://github.com/user-attachments/assets/4c602c90-e79b-4b09-8460-c1845d119fe4)

Practical Application Example 2
----
Explored the information with same senarions on the same dataset with coupon type CoffeeHouse.
Data Understanding  and cleanup.**
---
Same as above cleanup

Acceptance rate comparision (Under 25 and Above 25)
---
Drivers below 25 go to Coffee Shop:247

Drivers above 25 go to Coffee Shop:580

![image](https://github.com/user-attachments/assets/159d6c14-3b0c-4e3b-9566-e31f14df25e7)

Acceptance rate comparision (no kids,other than farming,went more than once to bar)
---
No Kids passengers go to the coffee shop : 16

No Farming passengers go to the coffee ship:16

More than once go to the coffee ship:17

               
![image](https://github.com/user-attachments/assets/017745c7-f97a-4df4-ab40-73ef09639ca7)

Acceptance rate comparision (under-30', 'no-kids-widow', 'bar more than 4 times -Income less than 50K)
---
Under 30 go to the conffee shop: 10

Other than window go to the conffee shop:  16

more than 4 times -Income less than 50K go to the Coffee Shop: 0

![image](https://github.com/user-attachments/assets/6ba2f4e9-8170-4981-9242-b71fb395014c)

Coupons Accepted/rejected for coupon type 'Coffee House'
---
Total number of Coupons for coupons type 'Coffee House' :108

Total number of Coupons accepted:62

![image](https://github.com/user-attachments/assets/d477740f-3ac1-4b61-8a72-c1ad3e1ab51f)



