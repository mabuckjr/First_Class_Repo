# Kickstarting with Excel

## Overview of Project
   This project involved helping a ficticious friend named Louise analyze Kickstarters of various types. The same set of data was used both in our activities courses, as well as our challenge assignment. I used different tools in Excel, from pivot tables and charts, statistical analysis formulas, formulas designed to clean up the data, and more to help me "make sense" of the data provided. All in all, I learned new skills and refined others through this example project. Louise should know **a lot** more about her data now! 
### Purpose
   For me, the purpose of this project is to ensure we know the basics behind each tool in excel. With this challenge now completed, I know that I can take the skills I learned here into my job and perform a more in-depth analysis of any dataset that is given to me from here on. I not only learned individual skills that will help me along my "excel journey," but I also learned how to combine these skills to sift down to a smaller amount of data that I truly want to analyze.
   
   For Louise, the purpose of the project was to understand many different aspects of Kickstarters. Sometimes, she wanted data about a specific type of Kickstarter (such as those related to Theater). Sometimes she wanted to know more about the data based on other paramaters, such as the geographic location of the kickstarter, the date it was created, or the fundraising goal. Sometimes, it was all three! She wanted to truly understand what made a kickstarter work, and I think my analysis will help her in her journey.
## Analysis and Challenges
   In this section I will break down how I was able to finish the first two deliverables for this challenge. Using different skills for each one, I was able to analyze the data in a new way, and hopefully help Louise understand how launch dates and fundraising goals can affect the outcome of a kickstarter campaign. For both deliverables, I was using the given data that I formatted in the "Kickstarter" Sheet found in the [Kickstarter Excel Workbook](https://github.com/mabuckjr/kickstarter-analysis/blob/main/Copy%20of%20Kickstarter_Challenge.xlsx). 
### Analysis of Outcomes Based on Launch Date
   For this deliverable, I started with the "Kickstarter" sheet. I converted the "Date Created Conversion" Column to a year using the YEAR() function. Then I created a pivot table in a new sheet that we named "Theater Outcomes by Launch Date." I then filtered the data based on the "Parent Category" and "Years." I populated the Columns field with "outcomes," Rows with "Date Created Conversion," and Values with outcomes again. I had to remove years and quarters from the rows field, as that is sometimes autopopulated when a date is put into a pivot field.
   
   Next, I filtered the columns to only shwo successful, failed, and canceled kickstarters. I further filtered the data by setting the Parent Category to "theater," which then will only show theater kickstarters in the table. I then sorted the column labels in ascending order so that successful kickstarters were shown first. With this final pivot table, I created a line graph. On the x-axis are months, and the y-axis has the outcome of the kickstarters. I then added a title to the graph, and we now have a great visual representation of successful, failed, and canceled theater kickstarters based on the month they were launched (see below): 
   
   [Theater Outcomes Based on Launch Data](https://github.com/mabuckjr/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png)
   
   I didn't have any challenges with this myself, but I could imagine that people could have had difficulties populating the fields on the pivot table. I often get confused by the idea of putting a pivot table field in both the column and values sections. If I wasn't familiar with pivot tables, I think that matching the formatting shown on Canvas could have been pretty difficult. 

### Analysis of Outcomes Based on Goals
   The next deliverable required me to create another new sheet called "Outcomes Based on Goals." In it, I created 8 columns (Goal, Number Successful, Number Failed, Number Canceled, Total Projects, Percentage Successful, Percentage Failed, and Percentage Canceled). In the Goal column, we created our 12 ranges for various dollar amounts that the kickstarters may have set for their goals. The first started at "Less than 1000," then "1000 to 4999," and then went up in 5000 increments from there until "Greater than 50000."
   
   I then used the COUNTIFS() function to populate the next three columns (Number Successful, Number Failed, and Number Canceled). Using data in the "Kickstarter" sheet, the COUNTIF() function allowed me to filter the "outcome," "goal," and "Subcategory" columns at the same time. I filtered "outcome" by successful, failed, or canceled; "goal" by the dollar amount ranges I listed above; and "Subcategory" as plays for our purposes.
   
   Then, I used the SUM() function to populate the "Total Projects" column with the different types of outcomes in each row. This made it easy to calculate the percentage for each outcome in the following 3 columns, finishing my table. I used the table to create another line graph titled "Outcomes Based on Goal," which helped me visualize how the initial financial goal of a kickstarter likely impacts the success rate of a kickstarter. See the graph below to see that relationship:
   
   [Outcomes Based on Goal](https://github.com/mabuckjr/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png) 
   
   In this deliverable, I had a lot of trouble initially with the COUNTIFS() function. I have used this function before, but in a much simpler setting than in this example. Once I practiced with it a couple of times, I was able to fully understand the syntax and replicate it accurately. The part that I was forgetting were the dollar signs in front of certain cell values to lock them in place. 

### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

   1) Over the years, the most successful month to launch a theater-based kickstarter has been May.
   2) Less than 3% of the theater-based startups have been canceled in our data set.

- What can you conclude about the Outcomes based on Goals?

   On average, plays that set kickstarter goals of more than $20,000 were more likely to fail than succeed. For the most successful kickstarter, my analysis would suggest that you should set your fundraising goal at $5,000 or less.

- What are some limitations of this dataset?

   It is hard to tell why successful kickstarters were successful, and why failed ideas were failures. For instance, if we wanted to explore the non-quantitative reasons for the outcome of each kickstarterin the subcategory "plays", we would need more qualitative information, reviews from critics, a list of popular actors and other cast members, theme/genre, and more to get an accurate idea of the "why."

   Another limitation is the scope of the geographic location. Sure, we know that some plays are in the US, GB, etc., but we all know that a touring play throughout all of California would be very different than a one-time show in Cleveland, Ohio.

- What are some other possible tables and/or graphs that we could create?

   We could sort the data differently for some of our existing tables (for example, sort by television instead of Theater for deliverable 1) and make many more descriptive charts, but those wouldn't be helpful for Louise.
   
   It would be interesting to continue making pivot tables comparing the outcome of a kickstarter to other parameters, like length of time that a kickstarter was active.
   
   Graphs comparing the outcomes of a category or sub-cateogry in different countries could help us understand what different populations like to give their money to across the globe.
