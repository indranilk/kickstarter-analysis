# kickstarter-analysis

Overview of Project

In this project we analyzed data of different campaigns. Using the dataset, we analyzed campaign outcomes based on launch date and funding goals. In the first part, we analyzed and designed chart based on theatre campaign outcomes such as which were successful, failed, and cancelled based on the dates they were launched. In the second part we analyzed and designed chart based on the percentage of successful, failed, and canceled plays with their funding goal amount. 

![image](https://raw.githubusercontent.com/indranilk/kickstarter-analysis/main/Resources/Theatre_Outcomes_vs_Launch.png)


Analysis and Challenges

This graph shows the outcomes of theatre based on the launch date. We first created a pivot table filtering parent category and years. We had to filter the column labels to display only the 3 possible outcomes such as successful, failed, and cancelled. After grouping the row label columns, it displayed each month of the year. The parent category data was filtered to show only the date for theater. The campaign outcomes were also sorted in descending order. We finally created a line chart from the table to show the relationship between outcome and the month campaign was launched. The blue line shows how many campaigns were successful, the orange shows how many failed and the grey showed how many were cancelled. The cancelled campaign outcomes remained very low throughout the year. Possible challenges that could occur are in getting the correct data filtered. It is possible that when creating the pivot table, some data doesn’t get copied over. The pivot table could have some missing fields and could miss important data such as possible outcomes, parent categories, or years. That would cause incorrect results and we would not get the correct number of successful, failed, or cancelled campaigns. 

