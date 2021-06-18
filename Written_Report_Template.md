# kickstarter-analysis


## **Purpose**
The purpose of this project is to provide insight on how the launch date and the goal amount of a crowdfunding campaign for theater affects its outcome.  

## **Analysis and Challenges**

### **Analysis of Outcomes Based on Launch Date**
To analyze outcomes based on launch date I created a pivot table that provided me with total numbers of succesful, failed and canceled campaigns for each month of the year. From this pivot table I created a line chart to visualize the change overtime. 

### **Analysis of Outcomes Based on Goals**
To analyze outcomes based on goals I created a new table and populated its cells using the COUNTIFS function. I then calculated the percentage of successful and failed campaigns. Using this table I created a line chart to visualize how successful campaigns are as the goal amount rises. 

This chart indicated an anomaly and to confirm it I created a column graph to highlight the huge concentration of campaigns in the lowest goal amounts. I then created another table populated by the data on the initial pivot table (Theater Outcomes Based on Launch Date) to measure the success rate for every month. 

### **Challenges and Difficulties Encountered**
The biggest challenge for me was the concentration of projects on one end of the goal spectrum. 

# **Results**

## **Outcomes based on Launch Date**


 ![](resources/Theater_Outcomes_vs_Launch.png)
 
 As we see in the graph there is parallel motion of both lines until they break apart in May to align again in August and to the end of the year. The margin increase between successful and failed lines combined with the increase in total campaigns translates to an increase in the success rate in late spring which holds for most of the summer. This indicates late spring and the first two thirds of the summer as the optimal period to start a campaign. As we move to the end of the summer success rates gradually fall and the margin between successful campaigns and failed is again locked in the initial parallel motion.  

We can verify this trend by taking in mind that most theatre projects require four to six months of planning, production and rehearsals. It is thus expected that more campaigns will start in late spring and early summer as they probably aim to conclude their campaigns early in the summer to premier in Fall. 

It is important to mention that although the number of campaigns created rises naturally in May due to the aforementioned circumstances, the success rate jumps by 5% which is the second biggest month to month increase. The biggest increase is observed from October to November where there is a 7% increase followed by a steep drop of 13% in December. This may represent a second wave of productions that aim to premier in the spring. 

![](resources/Success_Launch.png)

In the second graph we examine success rate based on launch date throughout the year. It is evident that the first six months of the year are more favorable for crowdfunding. By calculating the median for each half of the year we notice a 2% drop from first to second half. 

## **Outcomes based on Goals**

Observing the Outcomes based on Goals graph can be a real journey. As one would expect, we see a high concentration of successful campaigns in the low goal ranges of up to $10K. Then what follows is a natural and steady decline as the goal amounts rise. When we move past $30K this changes and we see the two lines trading places for a brief moment for amounts from $35K to $45K, before the successful line drops again in a real dramatic fashion. This anomaly is caused by a huge concentration of campaigns in the lower goal amounts and an, at best, scarce concentration of campaigns in the higher amounts. This is quite reasonable as projects with more ambitious goal amounts in excess of $30K would probably turn to other types of fundraising. Because of this I will consider every value 

## **Limitations**
This dataset needs further branching under the play subcategory. There are different factors within a theatre production that will affect the success of its crowdfunding campaign such as production duration, running time (how long will the play run for) , specific genre and theme (is it a Shakespeare play or is it a Mamet play ) and production location (indoor/outdoor).All these parameters would have allowed us to go in greater depths. 

Another limitation is the specifics on canceled campaigns. Because we do  not know the reason for the cancellations, we cannot include them when calculating averages. We do not know if a specific campaign was canceled because those running it realized they will never reach their goal or because of some random circumstance that forced them to this decision. If, for example, a campaign is canceled before its end date because it wasn't reaching its goal, then it should normally be counted as a failed campaign. 

### What are some other possible tables and/or graphs that we could create?

## **Outcomes based on Duration**
I think that the duration of a campaign also plays a big role in its success and so I created a sheet examining the relation between campaign duration and success. 

We also need a table breaking down campaign duration by amount
