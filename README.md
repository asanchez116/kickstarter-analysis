# Title: Kickstarter Module 1 Challenge: 
## 1.	Overview of the project:
## Background
An up and coming playwright wanted to start a crowd funding campaign to fund her newest play. After reviewing the data and taking the appropriate steps, the play came close to its fundraising goal in a short amount of time. 
## Purpose
Louise is now looking for an analysis to understand how different campaigns fared in relation to their launch dates and their funding goals. 
## 2.	Analysis and challenges: 

An analysis was conducted using the data-1-1-3-StarterBook.xlsx dataset. Time periods for variables “deadline” and Launched at” required transforming from unix time stamp to a readable format using an excel formula. Variable “Category and Subcategory” was separated into two variables for a parent category and a subcategory using Excel’s “text to columns”. Data for currency was reformatted to be easier for analysis. 
### Launch Date on Success
To investigate the impact of launch date on success of theatre projects, A pivot table was created filtering by parent category and years showing the number of cancelled, failed and successful kickstarter projects by month. The parent category was changed to show results for the “theatre” category. 

[![LDoTSTable](https://raw.githubusercontent.com/asanchez116/kickstarter-analysis/master/Resources/Screen%20Shot%202020-08-02%20at%208.22.21%20PM.png)](https://raw.githubusercontent.com/asanchez116/kickstarter-analysis/master/Resources/Screen%20Shot%202020-08-02%20at%208.22.21%20PM.png)
### Analysis of Goal on Success
To investigate the impact of kickstarter goal on success of kickstarter projects that were plays, a table was created to show the percentage of successful, failed, and cancelled play kickstarters whose goals fell within a specific monetary range. 

[![TOVL](https://raw.githubusercontent.com/asanchez116/kickstarter-analysis/master/Resources/Screen%20Shot%202020-08-02%20at%208.25.23%20PM.png)](https://raw.githubusercontent.com/asanchez116/kickstarter-analysis/master/Resources/Screen%20Shot%202020-08-02%20at%208.25.23%20PM.png)
Challenges that still exist include converting the currency types to be consistent.  
## 3.	Results:
### Conclusions from the Theatre Outcomes based on Launch Date
The proportion of successful theatre kickstarters appears to show an increasing trend for those launched during the middle of the year starting around March and peaking around May and June. After which counts of successful theatre kickstarters taper off when launched towards the end of the year. December is the least optimal time to launch a theatre kickstarter.   Failed theatre kickstarters show dramatically less variation by month compared to successful theatre kickstarters. 

[![TOVL](https://raw.githubusercontent.com/asanchez116/kickstarter-analysis/master/Resources/Theater_Outcomes_vs_Launch.png)](https://github.com/asanchez116/kickstarter-analysis/blob/master/Resources/Theater_Outcomes_vs_Launch.png)

### Conclusions from the Outcomes based on goals.
Overall, 66% of theatre kickstarters that were plays were successful vs 34% that failed. Overall, cheaper theatre kickstarters that were plays tend to be more successful with the proportion of successful theatre kickstarters that were plays steadily declining the higher the goals become. The exception is theatre kickstarters that were plays with goals ranging between $35,000 and $50,000 however, the n is comparatively small for this group. The quantity of kickstarters that were plays declines significantly the higher the goals become resulting in small numbers. Theatre kickstarters that were plays with goals between $5,000 and $24,999 are equally likely to be fail as they are to be successful.  
[![OBOG](https://raw.githubusercontent.com/asanchez116/kickstarter-analysis/master/Resources/Outcomes_vs_Goals.png)](https://github.com/asanchez116/kickstarter-analysis/blob/master/Resources/Outcomes_vs_Goals.png)

### Limitations of the dataset
Data varies in format for some variables (dollars vs pounds), there is some missing data for some time periods. For example, 2017 only had data for deadline only had data from January to May while launched at only had data for January through March for 2017. 
### Additional Graphs and Tables 
Additional graphs that might be helpful could include a look at comparisons of Kickstarter categories and subcategories by year to see if proportion of successful campaign categories/subcategories changes over years using a line graph. Using a line chart to plot the average percent funded by year filtered by subcategory and/or parent category. Showing a table ordered descending with the number of backers by category or by country to see if certain countries or categories might be better for different types of projects. 
