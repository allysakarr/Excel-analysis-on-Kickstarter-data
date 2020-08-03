# Excel-analysis-on-Kickstarter-data
## Overview of Project
My example client, Louise, originally wanted to start a crowd-funding campaign for her new play, *Fever*. Now that her fundraising has come close to meeting its goal relatively quickly, she is interested in seeing the results of other campaigns. Specifically, she wants to know how different campaigns compared to hers by looking at the different campaigns' launch dates and fundraising goals. 
### Purpose
The purpose of this project is to show the outcomes of these other campaigns to Louise in a visually understandable format so that she can know how her campaign for *Fever* compares to the results of other campaigns.
## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
In order to obtain an accurate reflection of other campaigns' outcomes based on launch date data, I found it best to create a pivot table with just the theater campaigns as that is the category relating to Louise's play. I set this pivot table up with the months on the rows portion of the table with the outcomes (successful, failed, or canceled) on the columns portio of the table to show the number of plays under each individual outcome over the progression of months. To view this table, please see the "Outcomes Based on Launch Date" sheet in this file: [Kickstarter_Challenge](https://github.com/allysakarr/Excel-analysis-on-Kickstarter-data/blob/master/Kickstarter_Challenge.xlsx?raw=true, "Kickstarter_Challenge).
I then made a line chart with markers to visualize the data to show Louise a monthly timeline (x-axis) and the trend of the number of plays (y-axis) throughout the months based on their outcomes. See image below: [Theater_Outcomes_vs_Launch](https://github.com/allysakarr/Excel-analysis-on-Kickstarter-data/blob/master/Resources/Theater_Outcomes_vs_Launch.png?raw=true, "Theater_Outcomes_vs_Launch") 
As Louise wants her play to succeed, we are going to concentrate on the number of successful plays for our analysis. According to this line chart, the peak of the line occurs around May with the values progressively going down after that month, meaning that the highest amount of successful plays occured in May. On the other hand, as the values begin to decrese, the number of successful plays reaches its lowest value, also noticeably lower than every other month, in December.
### Analysis of Outcomes Based on Goals
In order to determine which of the plays actually met their fundraising goals, I needed to re-format the data to divide up the actual goal amounts to display them properly with a visualization. I broke up the goal values into ranges in a separate sheet. I then calculated the number of plays with a successful outcome using these ranges with the data in the Kickstarter data sheet, specifically the goal amounts, the outcomes, and the specific "play" subcategory. I applied the same formula for the failed and canceled plays. I summed these projects and then used the number of a specific outcome divided by that sum to generate an overal percentage of plays with that specific outcome. I performed this action for all outcomes (successful, failed, and canceled). To see this work, please view the "Outcomes Based on Goals" sheet within this file: [Kickstarter_Challenge](https://github.com/allysakarr/Excel-analysis-on-Kickstarter-data/blob/master/Kickstarter_Challenge.xlsx?raw=true, "Kickstarter_Challenge) With these percentage values, I made a line chart displaying the percentages on the y-axis with the goal ranges on the x-axis to visualize the percentages of plays with a certain fundraising goal range were successful, failed, or canceled. See image below: [link](https://github.com/allysakarr/Excel-analysis-on-Kickstarter-data/blob/master/Resources/Outcomes_vs_Goal.png?raw=true "Outcomes_vs_Goal") 
According to the line chart, the percentage of successful plays was higher with the lowest fundraising goal range and the percentage of failed plays was lower with the lowest fundraising goal ranges. Conversely, the percentage of successful plays was lower with a higher fundraising goal range and the percentage of failed plays was higher with a higher fundraising goal range.
### Challenges and Difficulties Encountered
As I was creating the pivot table for the Outcomes Based on Launch data, I placed the "Data Created Conversion" table into the Axis (Categories) field, which then resulted in the years being listed in the rows portion of the table instead of months. In order to address this issue and make the data more pertinent for Louise to compare hers to, I deleted the "Quarters" and "Years 2" portions of the Axis field to reveal the launch months. I performed this action in order to give Louise an actual time of the year of when plays obtained certain outcomes. To address the outcomes portion of this pivot table, I placed the outcomes data in the Legend (Series) field, but the actual number of plays under the outcomes was not showing. I fixed this by placing the outcomes data also in the Values field in order to produce a count of the outcomes, providing an actual number value.  As I was developing the data to convert into a chart form for the Outcomes Based on Goals sheet, it was necessary to make every one of referenced columns absolute references in order to make sure Excel would not change the cell reference. In order to make the data reflect accurately on the visualization, I needed to change the axis to reflect the ranges on the x-axis and a percentage on the y-axis. 
## Results
To wrap up this analysis for Louise, I have come to a few conclusions. According to the campaign data analyzed in the Outcomes Based on Launch Date, the best month to launch a play would be in May as the number of successful plays is higher in that month. Conversely, the worst month to launch a play would be in December, which is when the number of successful plays is the lowest. So, Louise should launch a campaign in May for optimal fundraising to reach her goal. Speaking of her goal, according to the data on the other campaign's Outcomes Based on Goals, the plays with fundraising goals less than 1000 and from 1000 to 4999 were more succesful versus the other campaigns with higher fundraising goal ranges. I would recommend that Louise set her fundraising goal lower (somewhere between less than 1000 and 4999) in order to increase the likelihood of her play being successfully funded.  Despite the data yielding conclusive results, I did observe some limitations. The data did include many years of campaign data, and I would argue that using more current dates would be a better reflection of the current campaign fundraising sphere. Also, though Louise did want all of the campaign data, narrowing down this data further to just the US would localize more pertinent and similar campaigns to Louise's current campaign.
I did like using line charts to display this data, but I do see an opportunity to use other graphs to make the data more digestible. In the Outcomes Based on Launch Date chart, I find the number of plays to be a little harder to read on the y-axis, and potentially doing a bar chart could have represented these specific values better. But, since it is more of a time progression through the months, I would prefer the line chart for the x-axis values. In the Outcomes Based on Goals chart, the percentages and ranges are a bit more difficult to visualize in a line graph as the line graph seems more like a continuation of values vs individual values. I would have rather made a bar chart to reflect the individual range values and then showed the difference in the percentages that way.
