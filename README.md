# An Analysis of Kickstarter Campaigns with Excel
In this project, analysis was performed on Kickstarter data to uncover trends for Louise for better understanding.

## Overview of Project
Louise's play *Fever* was very close to meeting its fundraising campaign goal in a short amount of time. Other plays had variable outcomes to meeting their fundraising goals relative to their launch dates. Louise is interested in finding out how her campaign compared to others in this regard.
### Purpose
The purpose of this analysis is to provide a concise and straight forward visualization to Louise on campaign outcomes based on their launch dates and their funding goals to help her better understand how her play's fundraising campaign faired to others.
## Analysis and Challenges
Analysis was done on outcomes both based off launch date and fundraising goals. 
### Analysis of Outcomes Based on Launch Date
To provide proper visualization for analyzing the outcomes of the theater kickstarters, a pivot table was designed to filter only results pertaining to theater and the year campaigns were created. Since campaigns varied over many different years, it was decided that the data would be easiest to analyze by arranging it to dial down to the specific month of the year it was launched to get an idea of how the time of each year a campaign was launched would impact the outcome. Outcomes were then filtered to only show campaigns that were either successful, failed, or were canceled. Campaigns that are currently live were not displayed. A pivot chart line graph was then created to visualize the results and is shown below.

![Theater_Outcomes_vs_Launch](https://github.com/smyoung88/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
To provide succinct visualization of the outcomes based on campaign goals, a data table was created to breakdown the campaign goals into various increments of $5000 starting with $1000 and below all the way to greater than $50,000. For each incriment, the number of successful, failed, and canceled outcomes had to be determined only for plays by filtering the results based off of the goal increment, the specific outcome, and only play campaigns. Once this was completed, the total projects including each outcome was determined for each goal increment. Finally, the data were converted to figure out the percentages of each outcome relative to the total amount of projects for each goal increment and were then displayed on a line graph to show the outcomes based on goals as shown below.

![Outcomes_vs_Goals](https://github.com/smyoung88/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
In any large dataset, it is challenging to make sure that data being pulled is staying consistent throughout all analysis. When using formulas in spreadsheets that pull from specific cells, it was important to lock in certain rows or columns that needed to stay the same when using the same formulas for other columns to make sure each was giving the correct output. In this process, I noticed I locked in the full cell in some of the formulas instead of just the column which caused some of the data to look off. Proper QAQC was performed on all references to make sure the correct data was being visualized before proceeding.

## Results

**What are two conclusions you can draw about the Outcomes based on Launch Date?**
  1. The three most succesful months for theater campaigns were started in May, June, and July.
  2. Both successful and failed campaigns seem to follow the same trend throughout the year except during the summertime when started campaigns saw best success.
  3. Campaigns launched at the end of the year did not have as much success as those that started in the first 3 quarters of the year.
  
**What can you conclude about the Outcomes based on Goals?**
  1. When drilling down to the plays only subcategory out of all the theater kickstarters, it is of note that none of the campaigns were canceled.
  2. The most successful campaigns had goals of less than $15,000 with the exception of goals from $35,000 to $45,000 which both had success rates of 67%. The general trend of the overal dataset for plays is a decreasing success rate as the goal increases.

**What are some limitations of this dataset?**
  1. A major limitation of the dataset is that there are only a total of 158 total campaigns with goals greater than $10,000 and almost 900 projects less than $10,000. There is only one data point in the $45,000 to $49,000 goal range which is not statistically significant enough to make a decision on. Stories and trends change based off of how data is grouped. The amount of projects available for analysis above $10,000 are very little and not something I would feel comfortable comparing to.
  2. Another limitation of the dataset is that although there are nine years worth of data, only four of the years have at least 30 kickstarters worth of data. The years and respective theater kickstarters are as follows:
 <p align="center">
 ![Theater_Kickstarters_by_Year](https://github.com/smyoung88/kickstarter-analysis/blob/main/Resources/Theater_Kickstarters_by_Year.png)
 </p>
                           
  As seen, the most activity happened with theater kickstarters in 2014 through 2016.
    

**What are some other possible tables and/or graphs that we could create?**
  1. An important piece of the data could be the statistics behind each goal increment. Out of the total dataset, figure out how many outcomes are needed to be statistically significant and only include analysis on bins that had appropriate amount of projects in them. Decisions made on statistically insignificant data can be very risky. Instead of arbitrary $5,000 bins, let the statistics tell you what each bin size should consist of.
  2. I would also show percentage of success and failed campaigns by month. It is nice to see totals, but statistics can help make more concrete decisions if enough data is available.
  3. Another graph we could overlay even with the current graph is displaying the duration of the campaign alongside the outcome % graph.  There could be a trend for outcomes being more successful because it ran longer. The correlation might just be coincidence that certain launch months had more successful outcomes than others.
