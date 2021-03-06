# kickstarter_analysis

### Purpose
 The purpose of this project is to provide insight on how the launch date and the goal amount of a crowdfunding campaign for theater affect its outcome.  

## **Analysis and Challenges**

### **Analysis of Outcomes Based on Launch Date**

 To analyze outcomes based on launch date I created a pivot table that provided me with total numbers of succesful, failed and canceled campaigns for each month of the year. From this pivot table I created a line chart to visualize the change overtime. 

![](png/Theater_Outcomes_vs_Launch.png)

 As we see in the graph there is parallel motion of both lines and this indicates a steady success rate. The lines then break apart in March when we observe an increase in successful plays compared to failed plays which intensifies throughout April and reaches its peak in May. After that point successful campaigns slowly decrease while failed campaigns remain steady until the end of the year when the two lines almost meet . To be more precise regarding the actual change in success rate we have to create one more graph drawing data from the same table.   
  
  ![](png/suc_launch.png)
  
  There is a mostly gentle movement in this graph for the first nine months of the year before it hits turbulance in October. The average success rate for the first three quarters of the year is 64% while for the last quarter it is 57% .Highest percentage of success is observed in May and June at 67% and 68% respectively and the lowest in December at 51%. This may be attributed to **seasonal bias** as people tend to be more optimistic, extrovert and generous in the spring but more preoccupied with matters of their own at the end of the year when they also tend to spend more money in gifts and outings. There is no indication in the current data set of a more tangible cause for the fluctuation of success rate and **Launch Date does not significantly impact the outcome of a campaign** with the exception of a campaign that starts in the last quarter of the year. 

### **Analysis of Outcomes Based on Goals**

 To analyze outcomes based on goals I created a new table and populated its cells using the COUNTIFS function. I then calculated the percentage of successful and failed campaigns. Using this table I created a line chart to visualize  the number of successful campaigns  as the goal amount rises. 

![](png/Outcomes_vs_Goals.png)

 Observing the Outcomes based on Goals graph can be a real journey. As one would expect, we see a high number of successful campaigns in the low goal ranges of up to $10K. Then what follows is a natural and steady decline as the goal amounts rise. When we move past $30K this changes and we see the two lines trading places for a brief moment for amounts from $35K to $45K indicating a higher success rate for those campaigns. This alien conclusion highlighted the need for one more question and one more answer. What is the concentration of campaigns depending on the goal amount. 

![](png/density.png)

 As displayed in the graph above this anomaly is caused by a disproportionately high concentration of campaigns in the lower goal amounts compared to the scarcity of campaigns with higher goals . This is to be expected as projects with more ambitious goal amounts, in excess of $20K, would probably turn to other types of fundraising. In terms of visualization this imbalance prints as a misleading variation. 

 It is safe to disregard the visual results for campaigns with a goal amount higher than $20K and to conclude that as opposed to Launch Date, the Goal of a campaign can be defining. **There is a high propability of success for any campaign that sets a goal between $1K-$10K**. Chances decrease exponentially as goal amounts rise over the $10K mark. 

### **Challenges and Difficulties Encountered**

 One of the challenges was trying to understand why the first table on outcomes based on launch date is filtered in the parent category Theatre and not the subcategory "plays". Although the graph does not change significantly, we are including types of campaigns that could be irrelevant to our campaign .The second challenge was trying to detach myself from the things I think I know as a person who has worked in theatre for years. Every conclusion felt??arbitrary as I knew the dataset given is really insufficient as the variables that we are testing are not in reality defining for a campaign like this. 

### **Limitations**

 This dataset needs **further branching under the subcategory "plays"**. There are different factors within a theatre production that will affect the success of its crowdfunding campaign such as the specific genre and theme, indoor or outdoor production, and the one absolutely intangible variable; the vision each production has for the message it is carrying. This specific variable can be deciding and can make all the rest seem superficial.
 
 ## **Recommendations**
 
 One should expect that a crowdfunding campaign for a theatre play that starts in late March, with a modest goal amount of up to $10K would have the best chances to succeed. However, due to the specifics of the industry, no strategic choice can really guarantee any results if the core of the production - the vision - is not adequately developed. 


### **Further Research / Outcomes based on Duration**

 A useful addition to the already drawn conclusions could be provided by entering **duration** as a variable. Creating a new column on the spreadsheet, I subtracted *End Date Conversion* from *Launch Date Conversion* to count the days each campaign lasted. From this data I created a new table that includes goal amounts and duration to completion data. From this table we draw two more charts to display the relationship between Goal Amount and Duration as well as the Success Rate for each duration range. 

![](png/goal_time.png)

 This chart shows that there is no positive or negative correlation between goal amount and duration. A smaller goal amount does not guarantee a shorter campaign duration and vice versa. Month long campaigns show a success rate of 78%. 

![](png/suc_time.png)



