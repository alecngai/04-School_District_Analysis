# School District Analysis by Alec Ngai
## Project Overview

The school board has notified our client "Maria" that there has been academic dishonesty which has caused our analysis to be biased. We are required to replace the math and reading scores for Thomas High School 9th graders with NaN's, and repeat the school district analysis. We will use Anaconda to be able to read the data stored in CSV to analyze and present the data to the school board to allow for them to make further adjustments to their budgeting. 

1. Replace the math and reading scores for Thomas High School 9th graders. 
2. With the grades replaced we must re-do the analyis
    - The district summary
    - The school summary
    - The top 5 and bottom 5 performing schools, based on the overall passing rate
    - The average math score for each grade level from each school
    - The average reading score for each grade level from each school
    - The scores by school spending per student, by school size, and by school type

## Resources
- Data source: schools_complete.csv, students_complete.csv
- Software: Python 3.9.4, Visual Studio Code, 1.58.1, conda 4.10.1

## Results

### Old 
![District_Summary_Old](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/old_district_summary_df.png)

### New 

![District_Summary_New](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/new_district_summary_df.png)

After replacing the grades, we can take a look at how that affected the district_summary_df dataframe, here we have 9 metrics per school.
- Total Schools
    - This metric stayed the same
- Total Students
    -
- Total School Budget
- Per Studget Budget
- Average Math Score 
- Average Reading Score
- % Passing Math
- % Passing Reading
- % Overall Passing

## Summary