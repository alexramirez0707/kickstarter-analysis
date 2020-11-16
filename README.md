# Kickstarting with Excel


## Overview of Project
This project uses Excel to analyze Kickstarter campaign data. The data is used to visualize campaign outcomes based on their funding goals and launch dates.

### Purpose
Louise, our client, is a playwright interested in producing a play. She wants to use Kickstarter to crowdfund her campaign. She requested to perform an analysis using crowdfunding data of similar plays. The results produced by this report would ultimately help her determine if she should proceed with producing the play. 
This analysis will be conducted using Excel's formula functionalities, data filtering, and visualization tools.

## Analysis and Challenges:
 
### Analysis of Outcomes Based on Launch Date
**How the analysis was conducted:**
Data was filtered to focus on the outcomes of _successful, failed, and canceled_ Kickstarter campaigns. More specifically, only the parent category of _Theater_ campaigns was examined. Launch dates of the Kickstarter campaigns were also selected for analysis. Once all the data was filtered and chosen, it was then used to create a pivot chart. Pivot chart filtered by parent category and years (launch date). The outcomes were selected to fill the columns, the Launch date was selected to fill the rows, and the count of outcomes was selected to fill values. The pivot chart illustrates which months out of the year have the most successful outcomes and which months have the least successful campaign outcomes.

**Observation:**
The graph shows that the highest count of successful outcomes occurred between May and June, with a total of 211 successful campaigns (25% of the total successful campaigns). In contrast, the fundraising campaigns were the least successful in December, with only 37 (or 4%) successful campaigns.

The failed campaign outcomes did not show significant variation from month to month to conclude an accurate trend.

![](Resources/Theater_Outcomes_vs_Launch.png)


### Analysis of Outcomes Based on Goals
**How the analysis was conducted:**
For this analysis, fundraising goal amounts for plays are compared to evaluate their impact on a _successful, canceled, or failed_ outcome. The specific relationship examined is does the amount of the goal determine the outcome of the campaign.

The line chart is created by using the COUNTIFS function in Excel to produce a table. Columns of data such as Goal Amount, Outcome, and subcategory of _Plays_ are selected to produce a count of outcomes within each tier or threshold of the amount raised. To find the sum of total projects per goal tier, all outcomes per goal tier are added together. Each outcome number is then divided by the sum of total projects per goal tier, which produces a percentage. For example, of the total 180 projects with a goal amount of less than $1000, 141 projects have a successful outcome. This means play campaigns with a goal amount of less than $1000 are 76% successful.

**Observation:**
It was discovered that campaigns with a goal of less than $5000 are 74% successful. There are two goal tiers with amounts between $35,000 to $44,999, which showed 67% success. However, it should be noted that these two tiers only have a total of nine projects. The sample size is not large enough to accurately state whether the successful percentage would increase or decrease if more campaigns were within those goal tiers. Generally speaking, percentage of failed campaigns increased for goals greater than $5000.

![](Resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
1. I experienced slight difficulties in creating the pivot table. I could not instinctively place the right data fields in the correct columns and rows.
	+ To overcome my issue, I dragged multiple PivotTable fields around until my line chart matched the line chart in the module.

2. It is tedious and difficult to get `=COUNTIFS()` in every table cell correct. This was the most difficult part of the first two deliverables. I would mix up `">=" or "<="` within the formula which would produce the wrong number.
	+ 	To come this issue I used the `=COUNTIFS()`tutorial video in the module. I also asked my peers for recommendations on how to fix my formula.


## Results

_**Two conclusions that can be drawn about the Outcomes based on Launch Date are:**_
1. The months with the most successful outcomes are May and June, with a total of 211 successful outcomes. These two months contain 25% of the total successful outcomes, the highest percentage of any two months combined.
2. The month with the least amount of successful outcomes is December. There are only 37 successful outcomes in December. December has the worst successful to failed outcome ratio of all the months, 37 successful to 35 failed outcomes.

_**One conclusion that can be drawn about the Outcomes based on Goals is:**_
1. Any fundraising goal amount less than $5000 has a 74% chance of being successful. Success percentages decrease past that goal amount. It's not to say that a higher goal amount will not be successful. The data just suggests that as the amount of the goal increases, its odds of being successful decreases.

### Limitations of this dataset
1. This analysis only pulled data from Kickstarter. While Louise was primarily interested in launching her crowdfunding campaign on Kickstarter, I believe it may have been insightful to collect data from additional crowdfunding sites. Such as GoFundMe, Indiegogo, GoGetFunding, and Ulule to name a few.
2. Sample sizes were limited from month to month and year to year. In December for example, there were only 75 total count of outcomes. It is understandable that less projects in general are launched in December, but I believe collecting data from additional sites could have given a larger sample size for months that lacked campaign data.


### Possible tables and/or graphs that we can be created are:
1. I believe it would be beneficial to create a column within the Kickstarter sheet to see the _Duration of Campaign_. I'm curious to know if a short duration or deadline enables donors to act faster. Does a longer deadline cause contributors to donate at a slower rate?
	2. I think this information can be paired with donation incentivization 
