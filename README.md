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

### ***Old Disctrict Summary*** 
![District_Summary_Old](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/old_district_summary_df.png)

### ***New Disctrict Summary*** 

![District_Summary_New](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/new_district_summary_df.png)

After replacing the grades, we can take a look at how that affected the district_summary_df dataframe, here we have 8 metrics.
- **Total Schools**
    - This metric stayed the same
- **Total Students**
    - Went from 39,170 to 38,709
- **Total School Budget**
    - Budget stayed the same
- **Average Math Score**
    - The Average Math Score dropped from %79.0 to %78.9
- **Average Reading Score**
    - This value stayed the same
- **% Passing Math**
    - This also dropped from %75 to %74.8
- **% Passing Reading**
    - Dropped from %86 to %85.7 
- **% Overall Passing**
    - Dropped from %65 to %64.9

Here we can see the differences that dropping the 9th graders from Thomas High School had on the affect of the disctrict summary. 

### ***Old School Summary*** 
![old_per_school_summary](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/old_per_school_summary_df.png)

### ***New School Summary*** 

![new_per_school_summary](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/new_per_school_summary_df.png)

Everything stays the same except for Thomas Highschool, therefor lets take a close look at just them.

### ***Old Thomas School Summary*** 
![Old_Thomas_School_Summary](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/Old_Thomas_School_Summary.png)

### ***New Thomas School Summary*** 

![Old_Thomas_School_Summary](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/New_Thomas_School_Summary.png)

The main differences are 

- **Average Math Score**
    - The Average Math Score rised from %83.350937 to %83.418349
- **Average Reading Score**
    - The Average Reading Score decreased from %83.896082 to %83.84893
- **% Passing Math**
    - This also increased from %93.185639 to %93.272171
- **% Passing Reading**
    - Increased from %97.018739 to %97.308869
- **% Overall Passing**
    - Increased from %90.630324 to %90.948012 

As we can see from the results, the average reading score has decreased however, the rest of the metrics increased. We must take note that these changes are miniscule and hardly affect the results. 

### ***Top Five Schools based on overall passing*** 
![District_Summary_Old](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/top_five.png)

### ***Bottom Five Schools based on overall passing*** 

![District_Summary_New](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/bottom_five.png)

### ***The average math score for each grade level from each school*** 

![District_Summary_New](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/Average_Math_Scores.png)

### ***The average reading score for each grade level from each school*** 

![District_Summary_New](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/Average_Reading_Scores.png)

### ***The average reading score for each grade level from each school*** 

![District_Summary_New](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/Spending_Summary.png)

### ***The average reading score for each grade level from each school*** 

![District_Summary_New](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/Size_Summary.png)

### ***The average reading score for each grade level from each school*** 

![District_Summary_New](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/Type_Summary.png)

## Summary