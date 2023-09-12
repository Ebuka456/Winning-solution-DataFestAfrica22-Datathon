<h1 align="center">Winning Solution DataFestAfrica22 Datathon</h1>

<p align="center"> <img src="https://github.com/Ebuka456/Winning-solution-DataFestAfrica22-Datathon/blob/main/Final%20Round%20Analytics%20Datathon/Images/52438984779_9c319f2052_z.jpg" /> </p>

I participated in the DataFest Africa 2022 Datathon, assembling a team with diverse roles—a Data Analyst (my role) and two Data Scientists. The competition comprised three rigorous stages, evaluating our Data Science, Analytics, Problem Solving, and Presentation skills.

I'm pleased to announce that our team (Team Nova) emerged as the winners, showcasing the strength of our collective expertise and problem-solving abilities.

This readme would explain the steps taken to win the final round of the competition.

## 📗 Case Study

Every day, customers log their different types of complaints across their branches and expect quick responses and resolutions to their queries.
Some of these customers have a Service level agreement with the Network service provider to resolve their daily queries within a particular average duration. This service center has different Managers and operators looking into the customers' issues and Performance can be measured weekly and daily.
#### Manager’s Expectations:
- To provide a general outlook of the performance of the business based on relevant metrics.
- The top executives believe we should optimize TAT(Turn Around Time) between 6 pm to 9 pm every day due to backlash from disgruntled customers. Do you agree? Show us the data to support your position. Hint: Round-up time to start of the hour
- To highlight key factors leading to a delay in ticket response time(Normal response time: Within 10 secs?
- To highlight which managers and operators are performing well and which are struggling to meet up with the required resolution Time.

## 📗 Data Transformation (Cleaning)
For this analysis, all our transformations and datetime manipulations were done using Python and our visualization was done using PowerBI. We imported pandas and NumPy with their respective aliases. We converted to datetime using
pd.to_datetime() for easy manipulation. These were some of our observations on the datasets:
- Missing Fault type record: We found 526 missing records on the Fault type.
- 974 entries showed a 0-time difference between response and resolution , a snapshot of what these records looks like is shown below:

<p align="center"> <img src="https://github.com/Ebuka456/Winning-solution-DataFestAfrica22-Datathon/blob/main/Final%20Round%20Analytics%20Datathon/Images/Screenshot%202023-09-12%20094320.png" /> </p>

- The ticket close time had 639 empty cells. Since we did not need this for calculating any key metric, it was not included in our report.
- From our data, we had 1053 rows whose total response seconds were less than or equal to 10 secs. Out of which 974 showed a 0-time difference between response and resolution as earlier stated.

## 📗 Data Exploration and Visualization
Case Study Question 1: The general outlook of the performance of the business based on relevant metrics.
From the overview page, We had the following:

![](https://github.com/Ebuka456/Winning-solution-DataFestAfrica22-Datathon/blob/main/Final%20Round%20Analytics%20Datathon/Nova%20Report%20Image/Team%20Nova%20report_page-0002.jpg)

- There were 5998 recorded reports in December 2020.
- We observed 274 average response time(seconds) and 2.41 average resolution time(hours)
- There were 4 managers and 28 operators. 7 operators are assigned to a particular manager.
- 89.35% (5359) of Tickets are completed while 9.49% (569) are still active and 1.17% (70) are terminated.
- Social media is the most used report channel having 28.41% of our total reports.
- The most common fault type from the report received is from the customer's end. This was noticed among 52.53%(3151) of our reports.

To read the remaining part of the documentation to see how we answered the business questions, Continue reading [here](https://github.com/Ebuka456/Winning-solution-DataFestAfrica22-Datathon/blob/main/Final%20Round%20Analytics%20Datathon/Nova_Zentel_Documentation.pdf)

To view the interactive report, check [here](https://app.powerbi.com/view?r=eyJrIjoiNmY0OTQ1NWQtNGNmNi00NTE1LThiNTctOGRmMDM3ZTk4ZTU3IiwidCI6IjUwZDA2MjZhLTcwN2UtNDk2ZC1iOGU1LTIwYjk1NzA5MTYzZSJ9)

## 📗 Recommendations for improvements 
- The Manager in charge of the least performing operator, should be probed about the work ethics and well being of the operator, as well as the working condition in comparison to other operators.
- The least performing operator should be made aware of the poor performance which could serve as a motivation for an improved performance in January.
- In order to keep the team morale as high as possible, the operator with the top performance should be rewarded and recognized and also allowed to share their strategy used for adhering to the required benchmark.
- Operators have fixed managers. Perhaps a rotation such that struggling operators will get to work under top performing managers, this could improve the general Operator performance.
- As observed with the surge in reports within the 28th and 31st of Dec, 2020, and the over reliance on social media as the most preferred report channel, there’s a need to have more operators in order to handle the influx of reports through other channels in the future.
- An automated response scheme should be created for the most common type of complaints, this could help reduce the number of redundant reports the operators would have to respond to.

## 📗 Conclusion

- From the results outlined above, seeing as future explorative and prescriptive data analytics is key to the company’s growth and services, extra attention should be given to the data extraction pipeline for time based fields in order to mitigate data quality issues during the course of analysis or data entry.
- Also, in general, no operator met with the required Service Level Agreement, there might be a need to restructure the SLA or better still hire more operators and create automated responses on social media channels in order to filter out common reports, this would create a room for the operators to handle more pressing issues.

We believe we have been able to give reasonable insights and recommendations to justify the analysis carried out for this project.

**Skills I used for this competition**: Data Gathering, Data Assessing, Data Cleaning, Data Exploration (Exploratory Data Analysis), Data Manipulation, Data Analysis, Data Visualization, Dashboarding and Reporting, Data Storytelling. 

