# An Analysis of Kickstarter Campaigns

## Overview
 This project was undertaken to assist an aspiring playwright, Louise, with starting a kickstarter campaign for her play. Utilizing the initial analysis data, Louise's campaign for her play *Fever* came close to meeting its fundraising goal within a short period of time. Upon success, Louise requested for more data which will be discussed in detail in this report. 

### Purpose
The purpose of the analysis was to identify trends and understand the performance of previous campaigns based on the Outcomes, Goal amount and the Launch date. The below, new factors were analysed in detail after the initial success:
* Outcomes based on Launch date
* Outcomes based on Goal amount

## Analysis and Challenges

The dataset used contained data from 4114 campaigns spread across multiple categories and multiple countries. The category theatre had 1369 datapoints, out of which 1066 were for the subcategory plays. This category was used as the base for analysis. The initial analysis based on campaigns for plays in the US had revealed that the ideal would be to start the campaign around May, with a goal amount between 1500 to 5000 dollars. Based on request, this was further studied in detail to better understand the effect of launch date and goal amount on the success rate.

### Analysis of Outcomes Based on Launch Date
To understand the effect of launch date on outcome, a pivot table was created using the month of launch (isolated from the Launch Date) as the row label and outcomes as the column label. The 'live' campaigns were filtered out since they were not completed. This data was filtered specifically for 'Theatre' campaigns. An additional filter containing the year of launch was made available for further analysis, if required. A pivot chart with line chart type was created and the observerd data showed that the success rate was high during the summer months (May-July). The month of **May** had the highest number (111) of successful campaigns. Though there was a peak in the successful campaigns, there was no corresponding dip in the failed campaigns; however it was also observed that the month of initiation does not have a considerable effect on the failed or canceled campaigns suggesting that there were other contributing factors.

![Theatre_Outcomes_Vs_Launch](https://github.com/Dhanushree27/Kickstarter-Analysis/blob/2a0b980b2c340421923f0cc12bcf71142f98cc87/Resources/Theatre_Outcomes_Vs_Launch.png)

### Analysis of Outcomes Based on Goals
The ideal goal amount was identified during initial analysis, using statistical concepts mean and median. Since the mean value was skewed, the median data was considered as the better approximation and a range of 1500 to 5000 dollars was suggested. The data also suggested that campaigns that had a very high goal amount are likely to fail. The skewness in mean of successful campaigns suggested that there were a few successful high goal campaigns, but there might have been other factors influencing the success as most of the high goal campaigns had failed. ---
For further analysis, the goal amount was classified into bins with a difference of 5000 and the values were compared to better understand the effect of goal amount. It was observed that campaigns with goals less than 1000 had the highest success rate, followed by campaigns with goals between 1000 and 5000. For the mid range between 5000 to 25000, there were a equal number of failed and successful campaigns suggesting that there were other factors influencing the success or failure of those campaigns. Compared to successful campaigns, there were a higher number of failed campaigns for goals greater than 25000, except for the range 35000 to 45000 which displayed a higher sucess rate. Despite the success, it was not considered a representative sample of the population as the number of campaigns were comparitively low (~6).

![Outcomes_Vs_Goals](https://github.com/Dhanushree27/Kickstarter-Analysis/blob/2a0b980b2c340421923f0cc12bcf71142f98cc87/Resources/Outcomes_Vs_Goals.png)

### Challenges and Difficulties Encountered
Since the analysis was for plays in the US with a lower goal amount, there was considerable sample data to perform the analysis and arrive at a result. If the request had been for a higher goal amount, with the current sample set, it would have been difficult to arrive at a conclusive result since there were other variables influencing the success rate. 
Also, if the analysis had been for a different subcategory with relatively low data points, the result might have not been comprehensive.

## Results
From the analysis, it was observed that campaigns started during summer months had a higher success rate and there was a decrease in success rate for campaigns started in winter months. The month of launch did not have a considerable effect on failed or canceled campaigns suggesting that there were other factors influencing the failure rate.---
With respect to the goal amount, the detailed analysis corroborated the initial analysis. Campaigns with goals lower than 5000 had a higher success rate and campaigns with high goals, greaater than 25000, had a higher failure rate with a few outliers. ---
The dataset is limited in that it is limited to basic parameters of the campaign and does not provide more information on the kind of promotion, audience group it was intended for or other factors that could influence the success or failure of the campaign. It is limited in its ability to understand causes for anamolies. Also, it does not have sufficient data points for all categories.---
Also, a time-based chart using the years could have been plotted to understand the general trend and current popularity of the category. More time-based charts using the years would have also helped us understand whether the goal Vs pledged amount or the number of backers had changed over the years. 


