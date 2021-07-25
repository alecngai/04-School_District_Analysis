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

After replacing the grades, we can take a look at how that affected the district_summary_df dataframe, here we have 8 metrics.
- Total Schools
    - This metric stayed the same
- Total Students
    - Went from 39,170 to 38,709, this is becaused we removed the 9th graders from Thomas High School 
- Total School Budget
    - Budget stayed the same
- Average Math Score 
    - The Average Math Score dropped from %79.0 to %78.9, this is due to the cheaters in the 9th grade being removed.
- Average Reading Score
    - This svalue stayed the same
- % Passing Math
    - This also dropped from %75 to %74.8 due to the removal of 9th graders from Thomas Highschool
- % Passing Reading
    - Dropped from $86 to %85.7 
- % Overall Passing
    - Dropped from %65 to %64.9

Here we can see the differences that dropping the 9th graders from Thomas High School had on the affect of the disctrict summary. 

## Summary