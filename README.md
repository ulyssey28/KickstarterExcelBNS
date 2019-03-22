
# Kickstarter Analysis

Over two billion dollars have been raised using the massively successful crowdfunding service, Kickstarter, but not every project has found success. Of the over 300,000 projects launched on Kickstarter, only a third have made it through the funding process with a positive outcome.
Since getting funded on Kickstarter requires meeting or exceeding the project's initial goal, many organizations spend months looking through past projects in an attempt to discover some trick to finding success. 

# Process:

•	Used the Excel table provided, to modify and analyze the data of four thousand past Kickstarter projects to uncover some of the market trends.

•	Used conditional formatting to fill each cell in the “state” column with a different color, based on whether the associated campaign was "successful," "failed," "cancelled," or currently "live".

•	Created a new column at column O called “percent” funded that uses a formula to uncover the amount of money a campaign made towards reaching its initial goal.

o	Used conditional formatting to fill each cell in the percent funded column using a three-color scale. The scale starts at 0 with a dark shade of red, transitioning to green at 100, and then moving towards blue at 200.

•	Created a new column at column P called “average” donation that uses a formula to uncover how much each backer for the project paid (on average).

•	Created two new columns, one called “category” at Q and another called “sub-category” at R, which use formulas to split the “Category” and “Sub-Category” column into two parts.
 
o	Created a new sheet with a pivot table that analyzes the initial sheet to count number of "successful", "failed", "cancelled", and "live" campaigns per category.

	Created a stacked column pivot chart filtered by “country” based on the created table.

o	Created a new sheet with a pivot table that analyzes the initial sheet to count number of "successful", "failed", "cancelled", and "live" campaigns per sub-category.

	Created a stacked column pivot chart filtered by country and “parent-category” based on the created table.

•	Note: 
Dates stored within the “deadline” and “launched_at” columns use unix timestamps ( so we need to convert these timestamps into a normal date using a formula)

o	Created a new column named “Date Created Conversion”  using formula to convert the data contained within “launched_at” into Excel's Date format

o	Created a new column named “Date Ended Conversion” using formula to convert the data contained within “deadline” into Excel's Date format

o	Created a new sheet with a pivot table with column values based on “state”, and rows based on “Date Created Conversion” (based on the count of “state”, and filtered based on “parent category” and “Years”).

o	Created a pivot chart line graph that visualizes this new table.



# Additional 
•	Created a new sheet with 8 columns: Goal, Number Successful, Number Failed, Number Canceled, Total Projects, Percentage Successful, Percentage Failed, and Percentage Canceled

o	In the “goal” column, create twelve rows with the following headers...

	Less Than 1000

	1000 to 4999

	5000 to 9999

	10000 to 14999

	15000 to 19999

	20000 to 24999

	25000 to 29999

	30000 to 34999

	35000 to 39999

	40000 to 44999

	45000 to 49999

	Greater than or equal to 50000
 
o	Using the COUNTIFS() formula, counted how many successful, failed, and canceled projects were created with goals within those ranges listed above. Populate the “Number Successful”, “Number Failed”, and “Number Canceled” columns with this data.

o	Added each of the values in the Number “Successful”, “Number Failed”, and “Number Canceled” columns to populate the “Total Projects” column.

o	Using a mathematic formula, found the percentage of projects which were successful, failed, or were canceled per goal range.

o	Created a line chart which graphs the relationship between a goal's amount and its chances at success, failure, or cancellation.



