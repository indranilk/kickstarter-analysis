# kickstarter-analysis
								Written Analysis of the Results
								
Overview of Project

	In this project we analyzed data of different campaigns. Using the dataset, we analyzed campaign outcomes based on launch date and funding goals. In the first part, we analyzed and designed chart based on theatre campaign outcomes such as which were successful, failed, and cancelled based on the dates they were launched. In the second part we analyzed and designed chart based on the percentage of successful, failed, and canceled plays with their funding goal amount. 

![image](https://raw.githubusercontent.com/indranilk/kickstarter-analysis/main/Resources/Theatre_Outcomes_vs_Launch.png)


Analysis and Challenges

	This graph shows the outcomes of theatre based on the launch date. We first created a pivot table filtering parent category and years. We had to filter the column labels to display only the 3 possible outcomes such as successful, failed, and cancelled. After grouping the row label columns, it displayed each month of the year. The parent category data was filtered to show only the date for theater. The campaign outcomes were also sorted in descending order. We finally created a line chart from the table to show the relationship between outcome and the month campaign was launched. The blue line shows how many campaigns were successful, the orange shows how many failed and the grey showed how many were cancelled. The cancelled campaign outcomes remained very low throughout the year. Possible challenges that could occur are in getting the correct data filtered. It is possible that when creating the pivot table, some data doesn’t get copied over. The pivot table could have some missing fields and could miss important data such as possible outcomes, parent categories, or years. That would cause incorrect results and we would not get the correct number of successful, failed, or cancelled campaigns. 

![image](https://raw.githubusercontent.com/indranilk/kickstarter-analysis/main/Resources/Outcomes_vs_Goals.png)

  	This graph shows the percentage of successful, failed, and cancelled plays based on the funding goal amount. We had to first create dollar amount ranges for all the goal amounts. Using COUNTIFS() function and filtering outcome column on goal amount and subcategory column. The COUNTIFS() function helped find the number of successful, failed, and cancelled campaigns for the subcategory plays. We added all the three types of projects to find the total projects for each goal range. Then we calculated the percentage successful, failed, and cancelled. The line chart created on outcomes based on goal shows the goal ranges plotted against the percentage of successful, failed, and cancelled campaigns. The green horizontal line on the bottom shows the percentage of campaigns cancelled. The red line shows the percentage failed, and the blue line shows the percentage of campaigns successful. One challenge that I encountered while making this graph was including the correct values in the countifs function. I was having difficulty writing the following code in each cell to calculate the data between the ranges:
	
COUNTIFS(Kickstarter!$F:$F,"successful",Kickstarter!$D:$D,">999",Kickstarter!$D:$D,"<5000",Kickstarter!$S:$S,"plays")
	
	In the example above I was adding the range as Kickstarter!$D:$D,">999” and “<5000” which caused me to get 0 for the 1000-5000 range. I had to play around with the code to help me get the correct value for the range.

Results:

Conclusion for Theatre Outcomes:
  	For the theatre outcomes by launch date I see that the successful campaign data fluctuated highly towards middle of the year and then decreased towards the end of the year. The failed campaign outcomes stayed mostly the same throughout the year. I assume that in summer there was a lot of demand for watching movies/plays in theatres so that’s why the campaigns were more successful during that time. More people were available to go to theatres while there were summer holidays. After summer holidays were over, people didn’t have much time to go to theatres so the campaign results started going down.

Conclusion for Outcomes based on goals:
  	The cancelled campaigns always remained at 0%. The successful campaigns started off high for smaller range goals and then fluctuated downwards as the goal range increased. The failed campaigns started off low for smaller range goals and then fluctuated upwards as the goal range increased. As the goal range amount increased it might have been tougher to get money for the plays so the number of successful projects decreased eventually. 

Limitations of dataset:
	These graphs had some outliers. In the theatre outcome based on launch date data, the number of successful campaign outcomes for May and June are limitations/outliers. Those numbers are extreme values in the graph. In the outcomes based on goals data, the number of successful plays with goal less than $1000, between $1000 and $5000, and the number of failed plays with goal between $1000 and $5000 are also limitations/outliers. Those are extreme values in the graph as they are really far in value compared to others. 

Other possible tables/graphs:
	We could create additional charts such as campaigns with average donations, date launched, or percentage funded. 



