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
The analysis for this particular figure was done with several COUNTIFS() functions.
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
## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
