# An Analysis for Kickstarter Campaigns
Performing analysis on Kickstarter data to uncover trends
## Case Description
Louise wants to start a crowdfunding campaign for her upcoming play Fever. She has an estimated budget of $10,000. She wants to know what factors make a campaign successful in the U.S. and what is a reasonable fundraising goal. Louise is also interested in researching the musical campaign’s performance in Great Britain. In this data analysis project, excel was used to perform data analysis on a Kickstarter Campaign performance dataset. Key findings will be provided to help Louise plan her campaign and set it up for success.
## Analysis and Findings
- Made an initial check of the dataset and adjusted format and data types.
- Used pivot tables and pivot charts to check how well each category or subcategory performed in different countries

![Outcomes by Category Chart](https://user-images.githubusercontent.com/106395288/170766502-bbac4846-838e-4943-bd56-ea1bd02776e1.png)

![Theater Campaign Outcomes by Subcategory](https://user-images.githubusercontent.com/106395288/170765618-12d28343-e2f7-4f71-ba52-74b5db27f1ea.png)

- Identified the best months of launching a theater campaign with pivot chart

![Theater Campaign Outcomes by Launch Month](https://user-images.githubusercontent.com/106395288/170766601-f9f919db-339e-4dc7-a615-198faeee9b45.png)

![Theater Campaign Sussessful Rate](https://user-images.githubusercontent.com/106395288/170766645-adea8fcb-72a2-4a21-91f8-a03102d016ae.png)

- Performed descriptive analysis for the campaign goal and pledged amount in the theater-plays category by the campaign outcomes in the United States.
  * Found that failed campaigns have higher fundraising goals on average. However, the average pledged amount and median pledged amount for failed campaigns are much lower than the successful ones, which means some other factors lead to campaign failure.
  * Found that the mean of each subset distribution is around the 3rd quartile, which shows that the data follows similar distributions in each subset. 
  * The standard deviations are larger than the means, indicating that all the values blow mean are considered as "close" to the center. 
  * Also, some large values are driving the distributions. Standard deviations of successful campaigns are rough twice the IQRs. The failed campaigns have standard deviations about three times the IQRs. Some failed kickstarter campaigns have really high goals. 
- Filtered the dataset to extract kickstarter's performance in Great Britain's Theater market. Identified outliners in this data subset with a boxplot. And found that a reasonable fundraising goal for musical campaigns in Great Britain is around £2,000. 

![Musical Campaign Performance in Great Britain](https://user-images.githubusercontent.com/106395288/170766772-88727bf9-5ab9-482b-9b22-96b6e468ddb3.png)

## Key Takeaways
- Play campaigns have high successful rate in the U.S. 
- The best months for launching a play campaign would be May and June. 
- More data is needed to find out the factors that lead to campaign failure except for the high fundraising goal.
- As the musical campaign’s performance in Great Britain, Louise probably should set her campaign goal at £2,000.
