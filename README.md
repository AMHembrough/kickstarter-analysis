# Fundraising Campaign Outcomes Based on Launch Date & Fundraising Goal Amounts

## Overview of Project

### Overview

Using the provided Kickstarter dataset, we evaluated how fundraising campaign outcomes (i.e. successful, failed, canceled) are related to campaign launch date and fundraising goal amounts.  The analysis was conducted in excel using a variety of techniques such as inserting new columns, leveraging excel equations, pivot tables and pivot charts.  Graphis were created to illustrate the relationships between fundraising campaign outcomes and fundraising campaign start date and fundraising campaign goal amounts.  

### Purpose 

The purpose of this project was to determine how various fundraising campaigns performed in relation to fundraising campaign launch date and fundraising goal amounts.  

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

The first analysis examined how different fundraising campaign outcomes (i.e. successful, failed, or canceled) were related to fundraising campaign launch dates.  To conduct this analysis, a new column was created containing year of fundraising campaign start date.  We then created a pivot table that showed a count of fundraising campaigns by campaign outcome (i.e. canceled, failed, successful) and month of fundraising start date.  This pivot table was then leveraged to create a pivot chart to visualize the relationship between fundraising campaign launch month and fundraising campaign outcome.      

![Pivot chart](https://raw.githubusercontent.com/AMHembrough/kickstarter-analysis/main/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals

The second analysis examined how different fundraising campaign outcomes (i.e. successful, failed, or canceled) were related to fundraising goals amounts.  To conduct this analysis, the countifs() function was utilized to count the number of successful, failed, and canceled plays based on fundraising goal amount.  The =sum() function was then used to sum across all fundraising campaign outcomes for each of the fundraising goal amount ranges.  The percentage of fundraising campaigns that were successful, failed, or canceled across each of the fundraising goal amount ranges was then calculated using simple arithmetic.  A pivot chart was created to visualize the relationship between fundraising campaign goal amounts and fundraising campaign outcome.      

![Pivot chart](https://raw.githubusercontent.com/AMHembrough/kickstarter-analysis/main/Outcomes_vs_Goals.png) 

### Challenges and Difficulties Encountered

One of the challenges that I encountered was that my second graphic did not initially match the graphic provided in Bootcamp Spot.  I hypothesized that I had an issue with a filter, and tested this hypothesis by removing and then reapplying the correct filter.  This resolved my issue. 

## Results

### What are two conclusions you can draw about the Outcomes based on Launch Date?

Based on the analysis of this project, two conclusions can be drawn.
1. The majority of fundraising campaigns are launched in May and continue through the summer months. 
2. Fundraising campaigns launched in the summer months (especially May) are more likely to be successful than those launched outside of this window.  

### What can you conclude about the Outcomes based on Goals?

Fundraising campaigns with goal ranges less than $1,500 are the most likely to be successful.  

### What are some limitations of this dataset?

This dataset is limited by the following : 
- We only have 8 years of data.
- The most recent data are from 2017. 

### What are some other possible tables and/or graphs that we could create?

For the analysis of outcomes based on launch date, we could create a table / graph showing percentage of fundraising campaign outcomes based launch date (instead of count).  

For the analysis of outcomes based on fundraising goals, we could create a graph showing count of fundraising campaign outcomes based on fundraising goal (instead of %).
