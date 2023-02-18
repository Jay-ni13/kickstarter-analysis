# Kickstarting with Excel

## Overview of Project
A visual comparison of theater arts crowdfunding campaigns sourced from Kickstarter--a digital platform that organizes fundraising for creative projects--to investigate the relationship between project launch dates and their funding goals.

### Purpose
An up-and-coming playwright we previously assisted with tailoring a fundraising campaign for their US production of "Fever" and to whom we provided exploratory research on successful musical projects in Edinburgh and Great Britain requested additional analysis on how theater projects--successful, failed, or canceled--fared in relation to their launch dates and overall fundraising goals. 

## Analysis and Challenges
For this analysis, we began with a dataset of 4114 unique Kickstarter campaigns from 2009 to 2017. The dataset was further refined by category and subcategory to target projects specifically related to our client's interests.

### Analysis of Outcomes Based on Launch Date
To determine where certain projects succeeded or failed based on their launch date, we utilized Excel's conditional formatting to create a pivot table based on the 'theater' category and their date of creation in our dataset:

<img src="https://github.com/Jay-ni13/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_Table.png" width=70%>

The following line chart visualizes the relationship between the outcomes and launch months of the 1369 theater projects in our data subset:

![Theater Outcomes Based on Launch Date](https://github.com/Jay-ni13/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
To assess the fundraising goals of our dataset's 'plays' subcategory and their rate of success, failure, or cancelation, we created the following table utilizing Excel's =COUNTIFS() function:

![Outcomes vs Goals Table](https://github.com/Jay-ni13/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals_Table.png)

This line chart visulizes how the amount goal ranges relate to the percentage of successful, failed, or canceled plays projects in our data subset:

![Outcomes vs Goals Graph](https://github.com/Jay-ni13/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
One challenge of working with this dataset was the presence of several extreme data points. Within the 'theater' category were several large fundraising goals for theater-building proposals, whose target goals were much higher than your average play production. However, these data point fell within the SD and IQR of the overall dataset and had to be accounted for when analyzing goals. 
The extreme breadth of fundraising goals in this dataset also presents a difficulty when analyzing the percentage funded of a subset of projects (i.e. does a theater-production project with a goal-amount of $10 that achieves 1000% of its goal "do better" than a $1,000,000 theather-building project that only achieves 104% of its goal?).

## Results

### Outcomes Based on Launch Date
Two conclusions presented by analysis of theater project outcomes based on their launch date are: 
1) Projects launched in the months of May, June, and July have higher success rates than projects launched during the rest of the calendar year.
2) Launching campaigns in December and January--around the Christmas and New Year's holidays--has almost equal chances of failure or cancelation as they do of success.

### Outcomes Based on Goals
Analysis of the 'Outcomes Based on Goal' chart indicates that overall, theater projects with lower fundraising goals higher a higher success rate than projects with higher target goals.

However, the campaigns with a goal between $35,000-$45,000 deviate from this trend. As this range only includes 9 data points, it is hard to draw a definitive      conclusion except that this would be a useful goal-amount range to investigate when/if our playwright undertakes such a project.

### Limitations
Though this dataset contains 4114 unique data points, the analyses were based on subsets that contained only 1369 and 1047 data points (respectively). Likewise, the initial set included projects from 2009 to 2017, but the subsets only include data points from 2014 to 2017. As 2/3 of the initial dataset was not utilized in more targeted analyses, more datasets from other crowdfunding campaign platforms and sources would be useful in expanding the scope of this project and further refining its conclusions.

### Further Study
Other variables in this dataset that would be useful for expanding the scope of this analysis would be the length of time the fundraising projects were open and the number of backers for each campaign (i.e. a table that indicates how the number of backers relates to the amount of time a campaign is actively fundraising).
