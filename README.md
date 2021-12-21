# Kickstarting with Excel

## Overview of Project
The kickstarter project is intended to make informed recomendations based on available results from crowd funding campaigns to Lousie who desires to initiate a campaign to fund a play. The analysis was conducted using excel. The dataset used in the analysis contains 4113 results from previous campaigns. For each campaign, these data contain information on the date they were initiated, their outcome, the target and pledged amount of donations, the country of origin, and the category of the proposal. Exploratory data analysis was conducted to elicit attributes of these campaigns. Subsets of these data within the category of theater and with characteristics alligned with her campaign such as target goals was conducted for Louise. Informed by these analyses, Louise's campaign was able to accumulate the majority of the fundraising goal.        

### Purpose
In attempt to gain more understanding about the outcomes of related campaigns, Louise has requested further investigation. Using the parent category of theater, an analysis of the outcomes based of the launch dates was conducted. The purpose of this analysis is to reveal insight into the times of year which the most succesful outcomes occured. In addition to investigation of outcomes based on the launch date, analysis of the outcomes based on the fundraising goal was conducted. The purpose of this analysis is to use the subcategory of "plays" to determine if the amount of the fundraising goal attributed to the outcome of these campaings.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
The analysis based on the outcomes from the launch date was generated by extracting the year from the launch date. This was done using ```=YEAR(S2)``` where the cell S2 was the date formatted from the UNIX timestamp using ```=(((L2/60)/60)/24)+DATE(1970,1,1)``` where the cell L2 was the UNIX timestamp. After adding the year column, a pivot table was generated (Table 1). The pivot table filters for the year of the launchand the parent category. Populating the rows are the counts of the outcomes based on the month that they were initiated. Using these data, a line chart was generated to visualize the outcomes over time (Figure 1). This was done by inserting a line chart within excel. 

### Table1. Pivot table of kickstarter data filtered by the parent category of theater. 
| **Year Created**  | **(All)**     |        |          |             |
|:-----------------:|:-------------:|:------:|:--------:|:-----------:|
| **Parent Category**| **theater**  |        |          |             |
|                   |               |        |          |             |
| **Month**         | **successful**| **failed** | **canceled** | **Grand Total**|
| Jan               | 56            | 33     | 7        | 96          |
| Feb               | 71            | 39     | 3        | 113         |
| Mar               | 56            | 33     | 3        | 92          |
| Apr               | 71            | 40     | 2        | 113         |
| May               | 111           | 52     | 3        | 166         |
| Jun               | 100           | 49     | 4        | 153         |
| Jul               | 87            | 50     | 1        | 138         |
| Aug               | 72            | 47     | 4        | 123         |
| Sep               | 59            | 34     | 4        | 97          |
| Oct               | 65            | 50     | 0        | 115         |
| Nov               | 54            | 31     | 3        | 88          |
| Dec               | 37            | 35     | 3        | 75          |
| **Grand Total**   | **839**       | **493**| **37**   | **1369**    |

### Figure 1. Line plot of the theater outcomes by launch date
![Outcomes over time]("/Resources/Theater_Outcomes_vs_Launch.png")

Personal challenges that arose during this analysis pertained to the overall aesthetic of the line plot. Customizing the appearence to best visualize the data took time navigating the plot settings and finding the correct window to manipulate the plot features. Other possible challenges that one could be faced during this analysis is within the conversion of the UNIX timestamp. It is not immediately obvious to some who may be unfamiliar with the timestamp and it is not straightforward how to convert from seconds passed since January 1st, 1970 to the format of mm/dd/yyyy. 

### Analysis of Outcomes Based on Goals

### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
