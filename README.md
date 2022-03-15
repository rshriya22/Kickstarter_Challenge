# Kickstarter_Challenge



Overview of Project:

Kickstarter is an American public-benefit company that maintains world supporting platform which focused on the creativity of the people. It is the place where people share their creative ideas with the community where communities will together fund, and support creators and help creators to bring their projects into people’s life. 
The purpose of this project is to provide Louise with more information on her campaign outcomes based on their launch dates, funding goals. I use the given Kickstarter dataset to visualize the dataset. This will help Louise to understand her outcomes based on the album launching dates and their funding goals. This project will also help her to manage the fundraising goal in the future for her play Fever.


Theater Outcome Based on Lunch Date:

Analysis:

The new column, Years, in Kickstarter data is created where the Years() function is used to extract the data from the "Date Created Conversion" column. Adding the "years" column will analyze the outcome based on the lunch date and it also helps to know the years all the Plays were released.


 

After that, the Pivot table and pivot chart were created using the Kickstarter data set and placed the pivot table on the new sheet. The pivot table helps to analyze and explore many Outcomes in more detail. The pivot table was filtered based on the Parent Category, and Years and placed on appropriate fields in the columns, rows, and values. The column label is filtered to show only successful, failed, and canceled. Whereas the Parent Category is filtered to show the data for Theater only. The line graph from the pivot table was created to visualize the relationship between outcomes and launch a month after filtering and the "Parent Category and Theater" column.


 
 
 

Challenges: 

Some of the challenges and difficulties that I encounter: 
Before creating the pivot table and pivot chart. I need to add the “Years” column in the Kickstarter Data set. Not only does it help to know the total outcomes of launch dates that were created in a specific year, but it also helps to categorize total outcomes based on the month for all years. She uses the serial number for her Plays. So before creating the "Years" column, I create the “Date Create Conversion” in column S and “Date Ended Conversion” in column U to convert the serial number of “launch at” of column J and “deadline” of column I in date format.  
 
Another Challenge I encounter is to drag the Pivot chart fields in the Filters, Legends X-axis, and Value area. But I follow the direction to place the field in the right area. 


Outcome Based on Goals: 

Analysis

To find the outcome based on goal, the column of goal, number successful, number failed, number canceled, total projects, percentage successful, percentage failed, and percentage canceled were created in a new sheet. The data helps to visualize the column name based on the funding goal amount. Most of the amounts on this album have close or the same goal amount in the goal column. So the different row was made for a particular range of goal amount. It allows the group the project based on a certain range goal amount. Such as goals less than 1000, less than or equal to 4999 ……. 50,000 or more. After creating the columns, the COUNTIFS () function is used to calculate the "Number Successful," "Number Failed," and "Number Canceled" columns by filtering on the Kickstarter "outcome" column, on the "goal" amount column using the particular ranges and on the "Subcategory" column using "plays" as the criteria. Whereas Sum () function is used to find the total project for all three outcomes and =IFERROR () is used to calculate the percentage of successful, failed, and canceled projects for each row. Using the following data, the line graph is created to visualize the relationship between the goal-amount ranges on the x-axis and the percentage of successful, failed, or canceled projects on the y-axis.


Challenges: 

We need to select the “plays” category from the subcategory to find the outcomes of goals. But the Kickstarter datasheet has a “subcategory and category” column together in one column. So, it is hard to find the outcome only for the “plays category”. That is why the “subcategory and category” column is separated into two separate columns and named as “parent category” and “subcategory column”. Separating the column help me to find different types of goal outcomes. The row in "Number Successful," "Number Failed," and "Number Canceled" columns must be edited by a certain range on a goal amount.  I was getting error messages using the formula to find the outcomes based on the goals for those columns. Instead of typing the formula in each row of the column, I drag the formula and edit each row based on the range for goal amount based on the type of outcomes and the category. Such as for goal amount, less than 1000, I use the formula =COUNTIFS ('Kickstarter Analysis'!$D:$D,"<1000", 'Kickstarter Analysis'!$F:$F, "=successful", 'Kickstarter Analysis'!$R:$R, "=plays”.



Conclusion:

After looking at the pivot chart and graph of the Theater Outcomes by Launch Date, I find Louise should do the fundraising for her play “Fever” in May. It is because most of her plays are successful in May and there is less chance of play being canceled. 

Through the data from the Outcomes-based on Goals, I find most of Louise’s successful play goal amounts are less than 2000. It seems people do not buy the plays which are cost more than 5000. So, she could add the plays that are less than 2000 dollars. This way, she can earn more money and have the highest success rate for her plays. The data also shows none of her plays in the “plays” category were canceled. 

The Kickstarter data set is missing the artist’s name. If we know the artist for each category of the play, we will be able to find the popularity for the category based on the artist. 

We can also use the data set to analyze the data for the profit and loss she earns from a different category for her play. We should also use data to find what category of data has the highest success rate. It helps her to know the type of play that people love the most.

