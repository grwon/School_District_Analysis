# School_District_Analysis

## Project Overview
The school board has notified Maria and her supervisor that the students_complete.csv file shows evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. Although the school board does not know the full extent of the academic dishonesty, they want to uphold state-testing standards and have turned to Maria for help. She has asked you to replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. 

### Purpose
Purpose of this analysis is to determine how the replacement of grade 9 math and reading scores with NaNs for Thomas High School affected the overall analysis.

## Resources
- Data Source: students_complete.csv and schools_complete.csv
- Software: Python 3.8, Visual Studio Code, 1.46.1

## Results
The math and reading scores for grade 9 students in Thomas High School has been replaced with NaNs and the school district analysis was repeated. The below results and changes were noted.

### District Summary
- The district summary results show that:
    - there is no change to average math and average reading scores.
    - the passing percentage grade for Math, Reading and overall passing grade have all gone down by 1 percent compared to original analysis.
    
![District_Summary](https://github.com/grwon/School_District_Analysis/blob/master/Resources/district_summary_df.png)   

### School Summary
- The school summary results for Thomas High School show that:
    - there is no impact to the total and per student budget.
    - average math score went down from 83.418349 to 83.350937 after the grade 9 students' math scores were replaced with NANs.
    - average reading score also went up from 83.848930 to 83.896082
    - however, % of students passing math went down significantly from 93.27% to only 66.91%
    - similarly, % of students passing reading also went down significantly from 97.31% to only 69.66%
    - Overall passing % for Thomas High School went from 90.95% to only 65.08%

![School_Summary_Original](https://github.com/grwon/School_District_Analysis/blob/master/Resources/per_school_summary_df_tail_original.png)
![School_Summary_New](https://github.com/grwon/School_District_Analysis/blob/master/Resources/per_school_summary_df_tail_new.png)

### Ninth Graders' Math and Reading Scores
- Thomas High School's ninth graders' math and reading scores were replaced with NaNs, as you can see in the below pictures when compared to other school's performance.

![Ninth_Grade_Math](https://github.com/grwon/School_District_Analysis/blob/master/Resources/ninth_grade_math_scores.png)
![Ninth_Grade_Reading](https://github.com/grwon/School_District_Analysis/blob/master/Resources/ninth_grade_reading_scores.png)

### Other Impact
- When looking at Math and reading scores by grade results, only grade 9 column is affected. There is no impact to results for grade 10 to 12.

![Math_Score_By_Grade](https://github.com/grwon/School_District_Analysis/blob/master/Resources/math_scores_by_grade_tail.png)
![Reading_Score_By_Grade](https://github.com/grwon/School_District_Analysis/blob/master/Resources/reading_scores_by_grade_tail.png)

- See the new spending summary, scores by school size and scores by school type below.
![Spending_Summary](https://github.com/grwon/School_District_Analysis/blob/master/Resources/spending_summary.png)
![School Size_Summary](https://github.com/grwon/School_District_Analysis/blob/master/Resources/per_school_summary_school_size.png)
![Spending_Summary](https://github.com/grwon/School_District_Analysis/blob/master/Resources/type_summary.png)

## Summary
- This analysis has shown that there is questionable changes when comparing results with ninth grade math and reading scores replaced by NaNs. Major changes include average math score going down significantly and average reading score also went down from 97.31% to 69.66%. Other major change include Thomas High School is no longer in the top 5 school after the changes.
