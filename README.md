# Kickstarting with Excel

## Overview of Project
The kickstarter_challenge.xlsm file contains metrics about Kickstarter campaigns from 2009 - 2017. The key data columns are:
Goal: the currency value that the campaign needs to be successful
Pledged: the currency value the campaign actually recieved
Outcomes: Uses the text 'live' (ongoing campaign), success, failed, and canceled to denote the outcome of the campaign.
Date Created/Ended Conversion: Conversion of the UNIX timestamp to a standard MM/DD/YYYY format
Parent Category/Subcategory: enables filtering by the type of campaign

### Purpose
This project visualizes campaign outcomes in the Plays category based on their launch dates and their funding goals.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
The worksheet 'Outcomes Based on Launch Date contains a pivot table with the following fields in these areas.
Parent category is filtered by theatre. Outcomes is the pivot table column headings. Rows are merged into Month abbreviated by the first three letters. Values is the count of outcomes within the theater filter. Overall theater campaigns successfully reached their goals during each month of the year. The month with the most campaigns was May and the month with the least campaigns was December. Since May had the most overall campaigns, it also had the most failed and the most successful campaigns.

### Analysis of Outcomes Based on Goals
This worksheet breaks down the currency goals of Kickstarters filtered by the Subcategory 'Plays'. The rows are divided by the Outcome column in the Kickstarter worksheet. There are 1065 campaigns in this Subcategory. Campaigns with a goal between 1000 and 4999 were 73% successful, which is the highest percentage of success.



### Challenges and Difficulties Encountered
The UNIX Timestamp columns I/J had to be converted into MM/DD/YYYY format into columns S/T to create the Outcomes Based on Launch Date worksheet. The =Date() function was used.
The Text to Columns wizard was used to divide Column N, by the '/' into Column Q Parent Category and Column R Subcategory. This information was used to filter 'plays' goal data into Outcomes Based On Goals. Filtering is not possible without the date conversion and category columns. Both charts can be used to gain specific insights into the main kickstarter worksheet, so it's important to check pivot table filters in the Outcomes Based on Launch Date worksheet and the =COUNTIFS() criteria range.

## Results

A kickstarter campaign during the summer months from May to - July had more overall campaigns than the winter months from November - January. The percentage of successful campaigns in May was almost 67% while a campaign during the month of December had a 49% chance of being successful. Campaigns in the 'plays' subcategory that had a goal between $4999 and $9999 were the most successful and accounted for 50% of the succcessful projects.
The dataset only covers kickstarter campaigns from May of 2009 to August of 2017. There's no way to measure why supporters choose to pledge to a specific campaign category in any given year.
A pivot table could be created to demonstrate the average, mean, and mode of duration of a specigic category of campaigns. Another pivot table could show which categories by year/month.
A chart could be made that shows which year had the most campaigns overall. 
