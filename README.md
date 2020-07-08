# Costly Conversion : Pricing-Test


# **Problem Statement**

Company XYZ sells a software for \$39. Since revenue has been flat for some time, the VP of Product has decided to run a test increasing the price. She hopes that this would increase revenue. In the experiment, 66% of the users have seen the old price (\$39), while a random sample of 33% users a higher price (\$59). The test has been running for some time and the VP of Product is interested in understanding how it went and whether it would make sense to increase the price for all the users.

Especially need to answer the following questions:

1. Should the company sell its software for \$39 or \$59?

2. The VP of Product is interested in having a holistic view into user behavior, especially focusing on actionable insights that might increase conversion rate. What are your main findings looking at the data?

3.  The VP of Product feels that the test has been running for too long and she should have been able to get statistically significant results in a shorter time. Do you agree with her intuition? After how many days you would have stopped the test? Please, explain why.

# **Data**

Data includes two tables :<br>

1.   User_table - Information about the user.
2.   Test_results - Data about the test.

**Note**: For the purpose of the experiment, the group that sees the higher price is the experimental group while the one that sees the lower price is the control group.

# **Quick Answers**
1. *Should the company sell its software for \$39 or \$59?*
<br> <br>
Based on the result of the A/B testing, it is evident that the average revenue generated from the experimental group is greater than the control group(p-value <0.1*10^-8). Therefore, selling the software for \$59 would be good strategy. The control group's conversion rate is higher(1.99% v/s 1.556%) but presents lower average revenue per user relative to the experimental group. As revenue is the experimental variable in question as opposed to conversion rate, and thus it would be appropriate to increase the price.


2. *The VP of Product is interested in having a holistic view into user behavior, especially focusing on actionable insights that might increase conversion rate. What are your main findings looking at the data?*
<br>

>  User segments that were converted were : 
1.   Utilising Apple based products i.e. they were **MAC** and **iOS** users.
2.   Reaching the product via **Friend Referrals**.

> Surprisingly, that did not show much segementation in users that were converted as opposed to non converts was the choice of device used by them.

> In my opinion, optimising products for apple products and incentivizing friend referrals would be a good approach to maximize user groups that are likely to convert. Also, paying closer attention to groups that are least likely - **Linux** user may be a good utilisation not resources. My guess would be that the software maybe faulty when it comes to the Linux OS.

3.  *The VP of Product feels that the test has been running for too long and she should have been able to get statistically significant results in a shorter time. Do you agree with her intuition? After how many days you would have stopped the test? Please, explain why.*
<br><br>
Running the test for just **13 days** as opposed to 3 months resulted in p-value < 0.001 and therefore would have been sufficient to establish significant difference between the the average revenue of the two groups.
This was determined by calculating p-values for shorter time periods. By utilising the same A/B testing approach, it was checked whether running the A/B test for a shorter time period could still provide significant p-value. 
