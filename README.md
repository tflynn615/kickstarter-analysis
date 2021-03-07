# Kickstarting with Excel

## Overview of Project

This project analyzes outcomes of existing Kickstarter campaigns to identify what metrics correlate with successful fundraising. 

### Purpose

The client is interested in opening a new play in a US Theater, so the purpose of this project is to evaluate previous Kickstarter campaigns to determine what fundraising goals and traits are most likely to lead to raising sufficient funds. 

## Analysis and Challenges



### Analysis of Outcomes Based on Launch Date

I used a pivot table to compare total each campaign outcome against the month of campaign launch date filtered to only look at the Theater parent category. This was filtered to view only the successful, failed, and canceled results. This table was then made into a line chart to show the changes in each outcome over time:

![Theater_Outcomes_vs_Launch.png](Resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals

Next, I created a table that segmented campaign outcomes into segments based on fundraising goal amounts for only campaigns with the Play subcategory. These totals were found using the COUNTIFS formula to count the number of outcomes that met the goal range and the outcome segment (successful, failed, and canceled). Each of these segments were summed to find the total of projecets for each of the segments as well. The number of outcomes was then divided by the total projects for each goal segment to find the percentage of successful, failed, and canceled outcomes in the table. 

The table was then plotted on a line chart to demonstrate how the success rates change (y-axis) as the fundraising goal increases (x-axis): 

![Outcomes_vs_Goals.png](Resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered

I did encounter some issues understanding how the COUNTIFS formula could be used to capture a range of data, but after doing some research I found that the formula can handle multiple criteria because the syntax repeats itself as (range, criteria, range, criteria, etc). 

## Results


Evalutaing the Theater Outcomes by Launch Date, we can see that the highest number of successful campaigns started in the month of May and largely continue to decline through the rest of the year, excluding an uptick in the month of October. There is a combined uptick in successful and failed theater campaigns in the month of October, which is interesting since that is the only month of the year where there were no canceled campaigns. Because this data does not contain further insights into the fiscal year, I would be interested to see data around backers' budgeting cycles, as I wonder if this has any correlation with the trends that we are seeing here. It could also be beneficial to understand what is considered the Theater's "season" for running plays to understand if that is impacting the backers' decisions as well. 

Looking at the Outcomes by Goals, we can see that campaigns have a higher rate of success for goals that are less than $25,000. Above this amount, the rate of failure tends to increase. Because the data we have does not tell us how these campaigns intend to spend their fundraising goals, we do not know if the high dollar amount is the cause for the increase in failed campaigns. Here it could be valuable to explore the proposed budgets are for all Theater campaigns to see if those with goals above $25,000 are correlating with a high overhead amount that would lead to less confidence from backers. 

For further analysis, I would recommend charting campaign outcomes against the number of backers and the average donation amount. This could show correlation with whether it is better to seek many, small backers or one large backer in order to inform the client's strategy for fundraising outreach. 

