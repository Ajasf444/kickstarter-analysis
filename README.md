# Kickstarting with Excel

## Overview of Project

### Purpose
  The client, Louise, would like to have an analysis done on annual Kickstarter funding data to make a more informed decision on how to make the launch of a Kickstarter campaign for her play, * *Fever* *, successful.
To this end, Kickstarter campaign funding data for years ranging from mid 2009 to early 2017 were selected obtained and analysis was performed.
  
## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
![outcomes based on launch date](/resources/Theater_Outcomes_vs_Launch.png)

The figure above was generated via Excel as a pivot chart based off of a pivot table. 
This pivot table accumulated the outcomes of all Kickstarter campaigns categorized as the "theater" type sorted by their monthly launch date.
This chart easily allows one to visualize and interpret the monthly successes, failures, and cancellations of the campaigns launch dates.

### Analysis of Outcomes Based on Goals
![outcomes based on goals](/resources/Outcomes_vs_Goals.png)

The figure above was generated without the use of a pivot table.
The analysis for this particular figure was done with several `COUNTIFS()` functions.
As such the columns and rows were not readily available in the provided data so a few intermediate calculations had to be done to generate the necessary data for the figure.
This figure easily lets one view the percentage of successful, failed, and canceled play Kickstarter projects organized by their funding goals.

### Challenges and Difficulties Encountered
![outcomes based on launch date pivot table](/resources/Theater_Outcomes_vs_Launch_Pivot_Table.png)

The creation of the pivot table above was a challenging part for the analysis of the outcomes based on the launch date.
The default Kickstarter data doesn't have a column for months.
Fortunately, the month is contained in the start date for the campaigns.
Thus generating the months as rows was a relatively simple task.
All one has to do is group the rows by months as opposed to quarters.

![outcomes based on goals table](/resources/Outcomes_vs_Goals_Table.png)

The main difficulty in generating the table above was the arguments for the `COUNTIFS()` functions.
Much care has to be taken when adjusting the ranges manually, as it is incredibly easy to make a mistake in any one of the arguments.
Aside from that one could also have difficulty selecting the appropriate columns to plot in the table.
The simple solution is to hold the CTRL key and one can select non adjacent columns.

## Results

1. What are two conclusions you can draw about the Outcomes based on Launch Date?
   -May appears to be the best month to start a theater Kickstarter campaign.
   -In the month of December there are 37 successful campaigns and 35 failed campaigns. This would indicate that the probability that a theater Kickstarter campaign would get       funded if it started in the month of December amounts to a coin flip.

2. What can you conclude about the Outcomes based on Goals?
   -The probability for a play Kickstarter campaign getting funded appears to have approximately an 75% chance of getting funded as long as it is below $5000.
   -The $35,000 - $45,000 range for plays seems to have a 65% chance of getting funded, however this percentage could be misleading. There were only 9 campaigns started in those    price ranges over the course of the 9 year span. This low of a number of campaigns might not be enough to be indicative of the actual trend.

3. What are some limitations of this dataset?
   -A major limitation of this data set is that its latest year for data is 2017. 
   This is over a 3 year gap in data which could mean that for more recent Kickstarter campaigns the trends may no longer hold.
   Especially in light of the COVID pandemic the accuracy of the analysis for a Kickstarter campaign that would be starting more recently is likely to be low.

4. What are some other possible tables and/or graphs that we could create?
   -An interesting graph that one could make would be the percentage successful, failed, and canceled for theaters and plays but based off of the length of the campaign.
   There may be a certain length of time that is more advantageous to have a project get funded.
