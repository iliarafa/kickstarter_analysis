# kickstarter_ANALYSIS


## Purpose
The purpose of this project is to provide insight on how the launch date and the goal amount of a crowdfunding campaign for theater affects its outcome.  

## **Analysis and Challenges**

### **Analysis of Outcomes Based on Launch Date**
To analyze outcomes based on launch date I created a pivot table that provided me with total numbers of succesful, failed and canceled campaigns for each month of the year. From this pivot table I created a line chart to visualize the change overtime. From that pivot table I drew data to create another table to calculate mean and median values of campaign success rate based on launch date. 

### **Analysis of Outcomes Based on Goals**
To analyze outcomes based on goals I created a new table and populated its cells using the COUNTIFS function. I then calculated the percentage of successful and failed campaigns. Using this table I created a line chart to visualize how successful campaigns are as the goal amount rises. 

This chart indicated an anomaly and to confirm it I created a column graph to highlight the huge concentration of campaigns in the lowest goal amounts. 

### **Challenges and Difficulties Encountered**
The greatest challenge was the imbalance of campaigns throughout the goal amount field. I had to decide whether I could treat all data for amounts greater than 30K as outliers.  

# **Results**

## **Outcomes based on Launch Date**

![](png/Theater_Outcomes_vs_Launch.png)

  As we see in the graph there is parallel motion of both lines and this indicates a steady success rate. The lines then break apart in March when we observe an increase in successful plays compared to failed plays which intensifies throughout April and reaches its peak in May. After that point successful campaigns slowly decrease while failed campaigns remain steady until the end of the year when the two lines almost meet . This movement looks quite dramatic, but let's create one more chart to calculate the success rate based on launch date and see if it really is. 
  
  ![](png/suc_launch.png)
  
  
  There is a mostly gentle movement in this graph for the first nine months of the year before it hits turbulance in October. The average success rate for the first three quarters of the year is 64% while for the last quarter it is 57% .Highest percentage of success is observed in May and June at 67% and 68% respectively and the lowest in December at 51%. This may be attributed to **seasonal bias** as people tend to be more optimistic, extrovert and generous in the spring but more preoccupied with matters of their own at the end of the year when they also tend to spend more money in gifts and outings. There is no indication in the current data set of a more tangible cause for the fluctuation of success rate. 

 ## **Outcomes based on Goals**
 
 ![](png/out_goal.png)

Observing the Outcomes based on Goals graph can be a real journey. As one would expect, we see a high number of successful campaigns in the low goal ranges of up to $10K. Then what follows is a natural and steady decline as the goal amounts rise. When we move past $30K this changes and we see the two lines trading places for a brief moment for amounts from $35K to $45K, before the successful line drops again in a real dramatic fashion. 

As displayed in the graph below this anomaly is caused by a high concentration of campaigns in the lower goal amounts compared to the scarcity of campaigns with higher goals . This is to be expected as projects with more ambitious goal amounts, in excess of $30K, would probably turn to other types of fundraising. In terms of visualization this imbalance prints as a misleading variation. 

![](png/density.png)


 

## **Further Research Outcomes based on Duration**

![](png/goal_time.png)

A welcoming addition to the already drawn conclusions could be provided by entering **duration** as a variable. Creating a new column on the spreadsheet, I subtracted *End Date Conversion* from *Launch Date Conversion* to count the days each campaign lasted. From this data I created a new table that includes goal amounts and duration to completion data. From this table we draw two more charts to display the relationship between Goal Amount and Duration as well as the Success Rate for each duration range. 

From these we conclude it takes most succssful campaigns 30 days to reach their goal. Extending the campaign to 45 or 60 days will not bring in higher amounts. To support this we have to examine what was the duration for the high goal campaigns
![](png/suc_time.png)


## **Limitations**
This dataset needs **further branching under the play subcategory**. There are different factors within a theatre production that will affect the success of its crowdfunding campaign such as the specific genre and theme, indoor or outdoor production, and the one absolutely intangible variable; the vision each production has for the message it is carrying. This specific variable can be deciding and can make all the rest seem superficial. 

Another limitation is **the specifics on canceled campaigns**. Because we do  not know the reason for the cancelations, we cannot include them when calculating averages. We do not know if a specific campaign was canceled because those running it realized they will never reach their goal or because of some random circumstance that forced them to this decision. If, for example, a campaign is canceled before its end date because it wasn't reaching its goal, then it should normally be counted as a failed campaign. 
