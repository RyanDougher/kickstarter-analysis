# An Analysis of Kickstarter Campaigns

## Overview of Project

### Purpose

Louise would like to see how the launch date and goal amount effects the outcome of her campaigns. Using the Kickstarter data, Louise can gain insight into what months had the most amount of successful, failed, and canceled campaigns. Similarly, she can see if the goal amount has any correlation with the outcome. Using this information, Louise can make more informed decisions in order to increase the likelihood of her campaings success rate. 
## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

I created a pivot table to organize the data to show outcomes based on launch date. Launch date is represented in the rows and outcomes are represented in the columns. I then created a line chart to visualize this data more effectively.

![Theater_Outcomes_vs_Launch](/Users/ryandoougherty/Desktop/Data Analytics/Module 1 - Excel/resources/Theater_Outcomes_vs_Launch.png)

We can see that the month of May had the highest amount of successful campaigns, with June having the second highest. May also had the highest amount of failed campaigns, however the line for failed campaigns fluctuates far less than the line for succesful campaigns. The amount of successful and failed campaigns in December is nearly equal, with only 2 more successful campaigns than failed. The amount of canceled campaigns is low and has a small range of 3 to 7.

### Analysis of Outcomes Based on Goals

To analyze the outcomes based on goals, I organized the data into a tabular format, with the goal range in rows and outcome count and percentages in columns. To find the count of each outcome, I used the Countifs() function to filter for the appropriate goal range and "plays" subcategory. This was converted into a percentage in columns F through H.

![Outcomes_vs_Goals](/Users/ryandoougherty/Desktop/Data Analytics/Module 1 - Excel/resources/Outcomes_vs_Goals.png)

To visualize this data, I created a line chart. What we can see is that the majority of campaigns are successful for anything with a goal of $14999 or less. As the goal increases to $34999, most campaigns fail. From $35000 to $44999, Most campaings are successful again. And then the large majority of campaigns fail for anything higher.

### Challenges and Difficulties Encountered

The only challenges I faced was that repeating the Countifs() funtion on the outcomes based on goals analysis was tedious. By locking the ranges in the formula and copying/pasting, I was able to repeat this more efficiently. However, each goal range needed to be customized individually. The goal ranges also had a lot of repeating "0" and "9" digits, which made it easy to make a typo.

## Results

For outcomes based on launch, I concluded that the months of May through July have the highest success rate (May being the highest). The second conclusion is that December has the lowest success rate, with the amount of successful campaigns being just slightly higher than the amount of failed campaigns.

For outcomes based on goals, a campaign with a goal of less than $1000 has the highest success rate at 76%. A goal of over $45000 has the lowest success rate, ranging from 0% to 17%. A goal of $35000 to $44999 is a sweet spot with a fairly high success rate of 67%.

This data set is limited because we are analyzing launch date and goal separately. For example, its possible that May had the highest amount of successful campaigns because the average goal of the campaigns in May was low. We cannot see if launch date or goal amount has a stronger impact on the outcome.

To visualize outcomes based on goal, we could use a stacked column chart because we are comparing percentages of the outcomes. This could be a useful way to compare the amount of successful and failed campaigns.
