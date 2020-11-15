# Kickstarting with Excel


## Overview of Project
This project uses Excel to analyze Kickstarter campaign data. The data is used to visualize campaign outcomes based on their funding goals and launch dates.

### Purpose
Louise, our client, is a playwright interested in producing a play. She wants to use Kickstarter to crowdfund her campaign. She requested to perform an analysis using crowdfunding data of similar plays. The results produced by this report would ultimately help her determine if she should proceed with producing the play. 
This analysis will be conducted using Excel's formula functionalities, data filtering, and visualization tools.

## Analysis and Challenges:
 
### Analysis of Outcomes Based on Launch Date
Data was filtered to focus on the launch dates of successful, failed, and canceled Kickstarter theater campaigns. The pivot chart illustrates which months out of the year have the most successful outcomes and which months have the least successful campaign outcomes. The graph shows that the highest count of successful outcomes occurred between May and June, with a total of 211 successful campaigns (25% of the total successful campaigns). In contrast, the fundraising campaigns were the least successful in December, with only 37 (or 4%) successful campaigns.

The failed campaign outcomes did not show significant variation from month to month to conclude an accurate trend.

![](Resources/Theater_Outcomes_vs_Launch.png)


### Analysis of Outcomes Based on Goals
For this analysis, fundraising goal amounts for plays are compared to evaluate their impact on a successful, canceled, or failed outcome. The specific relationship examined is what goal amount has the highest percentage in both successful and failed campaigns. Louise is interested in comparing her crowdfund goal amount to similar plays. She would like to compare the results to predict if her campaign will be successful.

The line chart was created by using the COUNTIFS function in Excel to produce a table. Columns of data such as Goal Amount, Outcome, and subcategory of Plays were selected to produce a count of outcomes within each tier or threshold of the amount raised. To find the sum of total projects per goal tier, all outcomes per goal tier were added together. Each outcome number was then divided by the sum of total projects per goal tier, which produced a percentage. For example, of the total 180 projects with a goal amount of less than $1000, 141 of the projects had a successful outcome. This means play campaigns with a goal amount of less than $1000 were 76% successful.

Using the table and line chart, it was discovered that campaigns with a goal of less than $5000 were 74% successful. There are two goal tiers with amounts between $35,000 to $44,999, which showed 67% success. However, it should be noted that these two tiers only had a total of nine projects. The sample size is not large enough to accurately state whether the successful percentage would increase or decrease if more campaigns were within those goal tiers. Generally speaking, percentage of failed campaigns increased for goals greater than $5000.

![](Resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered


## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?


- What can you conclude about the Outcomes based on Goals?


- What are some limitations of this dataset?


- What are some other possible tables and/or graphs that we could create?
