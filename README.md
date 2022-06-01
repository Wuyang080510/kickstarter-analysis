# Kickstarting with Excel
# An Analysis for Kickstarter Campaigns

## Overview of Project
Louise wants to start a crowdfunding campaign for her upcoming play Fever. She has an estimated budget of $10,000. A dataset of past Kickstarter campaign performance was provided. An initial analysis was conducted. Louise got suggestions regarding fundraising goals and past performance of play campaigns. Now Louise’s play Fever came close to its fundraising goal. She wants to know how different campaigns performed based on their launch dates and funding goals. In this data analysis project, Excel is used to perform data analysis on a Kickstarter Campaign performance dataset. Key findings will be provided to help Louise plan her campaign and set it up for success.

## Analysis and Challenge
### Initial Analysis
- Made an initial check of the dataset and adjusted format and data types.
- Used pivot tables and pivot charts to check how well each category or subcategory performed in the U.S.
![U.S. Campaign Outcomes by Category](https://user-images.githubusercontent.com/106395288/171466017-367c29a1-3c17-416b-94f3-fbb096c0386d.png)

Most campaigns conducted in the U.S. are in the theater category. And theater campaigns had a high success rate.  


![U.S. Theater Campaign Outcomes by Subcategory](https://user-images.githubusercontent.com/106395288/171467909-c0e3e2c5-ccd0-4bf8-b3c9-b846cbd1cdab.png)

For the theater campaigns in the U.S., the play subcategory had the most campaign, and their success rate (61.4%) is much higher than the other two subcategories (46.9%).


### Analysis of Outcomes Based on Launch Date
- Extracted the year from the campaign’s launch date with Year () formula
- Created a pivot table of the theater campaign outcomes based on their launch date and visualized the data with a pivot chart

![Theater Outcomes Based on Launch Date](https://user-images.githubusercontent.com/106395288/171471173-7a109460-8a5d-40fb-b297-b1890ef6035d.png)

The number of successful campaigns in the theater category started to pick up in April and reached a peak in May. The number of failed campaigns is about the same in May and October. December has the lowest number of successful campaigns.


### Analysis of Outcomes based on Goals
- Grouped the goal amount into 12 groups
- Used COUNTIFS () function to calculate the number of successful, failed, and canceled play campaigns based on campaign goals

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/106395288/171475295-f929929b-33c4-4f11-8934-e046548cae0b.png)

The line of the percentage of successful campaigns started from a high number and dropped along the way to a lower rate in the goal range of $25,000 to $29,999. Then the successful rate started to pick up from the goal range of $30,000 to $34,999 and dropped to 0 in the goal range of $45,000 to $49,999. There are three intersections between the percentage successful line and the percentage failed line with a mirror reflection look.


### Challenge and Difficulties Encountered
In the first task of this assignment, I tried to use Year () function to extract the year part from the campaign created date. However, I kept getting "1995-07-07" and "1995-07-08" these two values rather than the year part of each date. I made sure the data type of the "date created conversion" column is DATE. I double-checked the function and the column and cell I referenced in the Year () function. The output kept the same. I tried to find out if someone else had the same issue as me. It seems like the wrong data type caused the problem. I noticed that the "Year" column has a data type of DATE. After I changed it to GENERAL, I got the correct output.

## Results
- May is the best month to launch a theater campaign throughout the year. 
- December is the worst month to launch a campaign. 
- Generally, lower campaign goals have a higher success rate. For lower campaign fundraising goals, campaigns with fundraising goals of less than $5,000 had the best performance. For higher campaign goals, $35,000 to $44,999 is a good range. 

### Limitations
More data is needed to find out the factors that lead to campaign failure except for the high fundraising goal.
Also, there are some extreme numbers in the campaign goal column. Further investigation is needed to determine if these are typos or if these are legitimate values that can be included in the analysis. 

### Recommendations
- Create a pivot table and a clustered column chart of campaign outcomes by average donation amount for different campaign categories. This table shows if the average donation amount affects the campaign outcome and which category of campaign tends to get a higher average donation amount.
- Create a pivot table of campaign outcomes by the number of donors for play campaigns to find out if there is a relationship between the number of donors and campaign results. Then, divide backers_count into four groups. Create a table with the campaign success rate and failure rate of different donor number groups to determine the optimum number of donors range for a successful campaign.
- A pivot table of the number of donors for each campaign category and a corresponding pie chart that show donor distribution among different campaign categories. 

