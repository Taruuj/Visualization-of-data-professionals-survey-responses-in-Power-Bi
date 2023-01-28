# Professional survey Power Bi visualizations

Data cleaning and visualization project in Power Bi on real data from a professional survey.

I started the project by cleaning the data using only Power Bi. I deleted the empty columns that I don't need for visualization (Columns E–I).
After this, I edit the columns that I use in the visualization. The modifications concern the columns that tell about the title, industry, country, favorite programming language, and yearly salary of the survey respondents.

I split the title, industry, country, and favorite programming language columns by delimiter. I use the delimiter "(" for title, industry, and country, and the delimiter ":" for favorite programming language. Then I remove the extra columns that were created.

Then I'll start working with the yearly salary column. I want to create a column with averages of the yearly salaries. First, I create a duplicate of the column. 

After this, I will split this column by digit, not non-digit. This creates 2 more separate columns, of which the last I will remove since it has only K letters in it. For the second column, I will get rid of the "K" and "-" values. I will do this by using the function for replacing values. I will also replace the value "+" with 225. After this, I will modify the remaining columns to be whole numbers.

After they are converted to a whole number, I can create a new column using the two columns. The custom column formula is: = ([#"Q3 - Current Yearly Salary (in USD)- Copy.1"]+[#"Q3 - Current Yearly Salary (in USD) - Copy.2"]) / 2. This creates a new column that contains the averages of the yearly salaries and can be used in the visualizations. Then I will again remove the extra yearly salary columns and leave the new custom column, which I will convert into a decimal number for visualization purposes.

Then I will move on to visualizations!
