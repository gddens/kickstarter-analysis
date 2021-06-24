# Kickstarter Campaigns Analysis Based on Launch Dates and Goals for Plays

## Overview of Project

### Purpose
The purpose of this project was to gauge how successful various Kickstarter campaigns for plays were based on their launch date as well as their funding goals. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
Created a pivot table using the date launched (separated by month) as the rows, the number of successful, failed, and canceled campaigns as the columns (with live campaigns filtered off), and the parent category for campaigns filtered to just "theater". This table was then used to create the below line graph comparing successful, unsuccessful, and canceled theater campaigns based on the launch date:

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/86032451/123244025-87592b80-d4b1-11eb-8b1e-d06c8a638e2a.png)

### Analysis of Outcomes Based on Goals
Manually entered a new chart and used formulas to populate data based on the number of projects that fall within a specific range of funding goals, and whether they were successful, failed, or canceled. The percentage of successful and failed campaigns was then calculated for each row, which was then used to create the below line chart:

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/86032451/123249588-1f0d4880-d4b7-11eb-953d-cb6dbf3e08df.png)

### Challenges and Difficulties Encountered
I did not experience any particular challenges with analyzing the first data set, although one could possibly have issues if specific data points aren't filtered off correctly (i.e., the rows isn't set to just months) creating a pivot table and accompanying chart that is far too wieldy to be useful for any sort of brief analysis. The second analysis proved to be a bit more difficult to get correct number for each range, since it was tempting to enter the formula based on how the goal columns were entered (i.e. only have the formula pull campaigns with a goal greater than 1000 and less than 4999), which meant I was excluding campaigns that could have been equal to either of those goals, and also meant that, since this pattern continued throughout the table, I also excluded campaigns that fell anywhere between highest number of one range and the lowest number of the next (i.e. anything between 4999 and 5000). I therefore had to adjust the formula so that each row had a range of greater than or equal to the lowest number in the range, and then less than the lowest number in the next range. An example of this would be formatting the row for goals with a range of 1000-4999 to pull campaigns that had a goal that was greater than or equal to 1000 but less than 5000, which is where the range in the row below it starts. 

## Results

- Two conclusions I can draw from Outcomes based on Launch Date is that the spring and summer months had the highest peak of successful theater campaigns, with May having the highest number overall. However, the number of failed theater campaigns also mirrored this trend, so an additional conclusion is that these months just had the highest overall number of campaigns.

- What I can conclude from Outcomes based on Goals is that an inverse relationship exists between funding goal and success rate - the lower the funding goal, the greater percentage it had of successful campaigns. However, it is not a perfect correlation, as a bump exists where successful campaigns again started outnumbering unsuccessful campaigns within the $35,000-$44,999 range. 

- Some limitations of this dataset are that Theater Outcomes by Dates only has overall number of campaigns, which makes it difficult to determine whether the higher number of successful campaigns in the spring and summer months is due to anything other than there being a higher overall number of campaigns during that time. It could also be too wide of a scope, as it looks at the overall theater category rather than just plays.  The Outcomes Based on Goals analysis is limited in that it only gives quantitative data (the funding goal), which does not help explain why the inverse relationship is interrupted when it comes to plays with a funding goal between $35,000-$44999 (i.e., whether these campaigns were launched by popular playwrights that were known to have more-expensive productions, and therefore were more likely to be successful in their fundraising campaigns because of that).

- An additional table/graph to help increase the effectiveness of this analysis could be one that looks at the percentage of successful theater outcomes based on launch dates, since it is hard to determine with the current table and graph if certain months were more successful due to anything other than there being a greater overall number of campaigns at the time. It may also be helpful to narrow that table/graph to just the "plays" sub-category so that it is more tailored to the client's needs.
