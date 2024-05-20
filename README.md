# Call-Center-KPI-Analysis(Using Power BI)

INTRODUCTION

 I applied for an online internship with PWC, through forage.

It was an exciting experience, the goal was to lay hold on real-time dataset and come up with insights for the assumed companies.

The call center dataset was made up of 5000 records, and 10 fields in all.

You can check out the dataset here

PROBLEM STATEMENT

And my assignment was to

“Create a dashboard in Power BI for Claire that reflects all relevant Key Performance Indicators (KPIs) and metrics in the dataset.”

To begin the analysis and then create the dashboard, after looking into the dataset, the fields and the values, and understanding what it was all about, I had questions about the dataset like

•Who was the most effective agent and why

•What day of the week did the company have the highest number of calls and why

•What month did the company record the most answered and resolved calls
•What was the most reason for clients calling in and how effective was the call
•What was the average speed of calls answered
•Which month did we have the least and most average satisfactory rating and why.

SKILLS DEMONSTRATED
Skills used in this analysis includes:
•Data cleaning
•DAX Function
•Data visualization
•Data analysis

DATA SOURCING
This dataset was provided by PWC internship unit, for the purpose of practice. By downloading it from the website it was obtained. It’s a dataset with one table and no related tables

DATA TRANSFORMATION

First of all, I loaded my data into power-Bi, I have used Power Query for the Data Cleaning. I highlighted the entire range and checked for duplicate record, none was found.

I proceeded to change the date type of the fields accordingly, for the date field, i notice the date were all imputed in text. I had to use the Data value function in other to change the text to date format.

I further proceeded to load my data into Power BI, it was clean enough for me so i didn’t need any further formatting in the query.

I created two calculated columns, one to get my Days as digits and the the other to get the full names of the days

***for_the_digits***
Day=weekdays(sheet1[Date].[Day])

***for_the_name_of_days***
Days=Format(sheet1[Day],"dddd")

I proceeded to write out a calculated measure, to obtain the average talk duration, excluding the rating that were 0, so as to get an accurate analysis.

Avg satifactory rate= Calculate(average(sheet1[sactifaction rating]),sheet1[sactifaction rating]<>0)
 
VISUALIZATION
Moving on, the dashboard was created still using Power BI, by the use of charts and graphs


The report is a single interactive dashboard
You can interact with the dashboard here

ANALYSIS

A Total of 5000 calls were recieved by the call center in the space of 3 months, January-March 2021.

1) 4054 were answered the remaining 946 were not,
and about 3646 complaints were resolved, they had their highest call-in and resolved calls in January.

2)Reason for calling
For the reason of the calls, it was observed that most of the callers called in for streaming complain out of the 5 reasons stated

3)Though majority of the complain about streaming were made in the January record, while the February and March had Admin support and Payment topping their list respectively.

It’s observed that the company had an improvement in streaming. But yet the company needed to work on their technical support system, they seem to be having consistent high complain for the space of the three months.

Call by Month


Most of the calls out of the 5000 calls in the three months came in in January, a total of 1772, out of which 1455 were answered and 1311 resolved.

But in February, there was a minor drop in number of call-ins but a large decline in the answered and resolved calls. The problem with February could be traced to the most complaint of the month -Admin support.

But gracefully, a fair improvement was noticed in the following month, the company was able to recover in the following month. They had a total of 1612 call in, 1301 answered and 1174 resolved.

More information would be needed for further findings about the company

Calls by Date and Weekday


Most of the calls were made on the weekday, Monday.

And the highest number of calls came in on the 11th of January with a total of 84 call-ins, majority of the reason for calling were payment.

Calls by time of the day


Between the hours of 11:30am and 3:30pm are generally times the call center recieve the most incoming calls from client

Most effective agent


Agent Jim was observed to be the most effective agent within the three month of function. He was effective not only to answer calls but most importantly to resolve the problems at hand and such agent should be considered for retainment. Also Dan was a seen as a good fit next to Jim. Most of the agent like Stewart is observed to require training on how to communicate and meet the necessary needs of the client, because he was able to answer a good number of calls but with a little number of resolved calls.

Average satisfactory rating


For the three month, average satisfactory rating of 3.40 was calculated. With the highest average in the month of Jan (3.45), then Feb (3.38) and Mar(3.37).

I noticed that there was a fall in satisfactory rating in February, could be attributed to the percentage of resolved calls to answered call in that month. But in March an improvement was made, though the average is still below the initial, but the difference between the resolved call of February and March is significant.

CONCLUSION
The call center experienced down time in the second month of the year, their efficiency was to be questioned. Though it was observed that in resolving the issues of their client, they had a fair rating.

I’ll recommend more training for the agents so as to improve in resolving calls and not only answering the calls, because generally most of the calls in the call center were answered without resolving


