# Kickstarting with Excel

## Overview of Project
   -This project involved helping a ficticious friend named Louise analyze Kickstarters of various types. The same set of data was used both in our activities courses, as well as our challenge assignment. I used different tools in Excel, from pivot tables and charts, statistical analysis formulas, formulas designed to clean up the data, and more to help me "make sense" of the data provided. All in all, I learned new skills and refined others through this example project. Louise should know **a lot** more about her data now! 
### Purpose
    -For me, the purpose of this project is to ensure we know the basics behind each tool in excel. With this challenge now completed, I know that I can take the skills I learned here into my job and perform a more in-depth analysis of any dataset that is given to me from here on. I not only learned individual skills that will help me along my "excel journey," but I also learned how to combine these skills to sift down to a smaller amount of data that I truly want to analyze.
    -For Louise, the purpose of the project was to understand many different aspects of Kickstarters. Sometimes, she wanted data about a specific type of Kickstarter (such as those related to Theater). Sometimes she wanted to know more about the data based on other paramaters, such as the geographic location of the kickstarter, the date it was created, or the fundraising goal. Sometimes, it was all three! She wanted to truly understand what made a kickstarter work, and I think my analysis will help her in her journey.
## Analysis and Challenges
   -In this section I will break down how I was able to get the first two deliverables for this challenge. Using different skills for each deliverable, I was able to analyze the data in a new way, and hopefully help Louise understand how launch dates and fundraising goals can affect the outcome of a kickstarter campaign. For both deliverables, I was using the given data that I formatted in the "Kickstarter" Sheet found in the [Kickstarter Excel Workbook](https://github.com/mabuckjr/kickstarter-analysis/blob/main/Copy%20of%20Kickstarter_Challenge.xlsx). 
### Analysis of Outcomes Based on Launch Date
   -For this deliverable, I started with the "Kickstarter" sheet. I converted the "Date Created Conversion" Column to a year using the Year() function. Then I created a pivot table in a new sheet that we named "Theater Outcomes by Launch Date." I then filtered the data based on the columns labeled "Parent Category" and "Years." I populated the Columns field with "outcomes," Rows with "Date Created Conversion," and Values with outcomes again. I had to remove years and quarters from the rows field, as that is sometimes autopopulated when a date is put into a pivot field.
   -Next, I filtered the columns to only shwo successful, failed, and canceled kickstarters. I further filtered the data by setting the Parent Category to "theater," which then will only show theater kickstarters in the table. I then sorted the column labels in ascending order so that successful kickstarters were shown first. With this final pivot table, I created a line graph. On the x-axis are months, and the y-axis has the outcome of the kickstarters. I then added a title to the graph, and we now have a great visual representation of successful, failed, and canceled theater kickstarters based on the month they were launched (see below): 
   [Theater Outcome vs. Launch]( kickstarter-analysis/Resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals

### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
