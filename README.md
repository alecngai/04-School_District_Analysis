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

![New_Thomas_School_Summary](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/New_Thomas_School_Summary.png)

The main differences are 

- **Average Math Score**
    - The Average Math Score decreased from %83.418349 to %83.350937
- **Average Reading Score**
    - The Average Reading Score increased from %83.84893 to %83.896082
- **% Passing Math**
    - This also decreased from %93.272171 to %93.185639 
- **% Passing Reading**
    - decreased from %97.308869 to %97.018739
- **% Overall Passing**
    - decreased from %90.948012 to %90.630324

As we can see from the results, the average reading score has increased however, the rest of the metrics decreased. We must take note that these changes are miniscule and hardly affect the results. 

### ***Top Five Schools based on overall passing*** 
![Top_Five](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/top_five.png)

### ***Bottom Five Schools based on overall passing*** 

![Bottom_Five](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/bottom_five.png)

There was no changes due to the fact the change in scores did not change much there for did not affect overall passing metric

### ***The average math score for each grade level from each school*** 

![Average_Math_Score](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/Average_Math_Scores.png)

### ***The previous average math score for each grade level from each school*** 

![Average_Math_Score](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/Old_Average_Math_Scores.png)

### ***The average reading score for each grade level from each school*** 

![Average_Reading_Scores](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/Average_Reading_Scores.png)

### ***The previous average reading score for each grade level from each school*** 

![Average_Reading_Scores](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/Old_Average_Reading_Scores.png)

As you can see these are exactly the same except for Thomas High School Grade 9 value is all NaN for both reading and math for the new analysis. 

### ***The scores by school spending per student*** 

![Spending_Summary](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/Spending_Summary.png)


### ***The previous scores by school spending per student*** 

![Spending_Summary](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/Old_Spending_Summary.png)

The only change is the decrease in %0.1 in both %Passing Reading and % Overall passing in the $630-$644 range, as no other values was changed and thomas high resides in this spending range. 

### ***The scores by school size per student*** 

![Size_Summary](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/Size_Summary.png)

### ***The previous scores by school size per student*** 

![Size_Summary](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/Old_Size_Summary.png)

There is a decrease of %0.1 percent in % Passing readings, in the medium school size, the rest are unaffected.

### ***The scores by school type per student*** 

![Type_Summary](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/Type_Summary.png)


### ***The previous scores by school type per student*** 

![Type_Summary](https://github.com/alecngai/04-School_District_Analysis/blob/main/Resources/Old_Type_Summary.png)

There is no change between the two analysis. 

## Summary

The changes are quite minor, there is mostly a decrease in average scores, this is probably due to the inflated grades of the cheaters in the 9th Grade of Thomas Highschool. 

The grades were already quite high for Thomas High School so there was no change in ranking in which school is the best by overall passing. 

The average math and reading scores are the same except for the 9th grade holding NaN values. 

For the scores by school spending, size, and type there are also miner changes of %0.1 percent, only in the ranges where Thomas Highschool excisted which is $630-$644, Medium and Charter.

In conclusion, removing the 9th Graders marks to re-run the analysis shows that it did not change much at all, we can conclude that majority of the 9th graders probably did not cheat and it was one or two outliers, as the scores match the average scores of other grades and there was not much difference. 