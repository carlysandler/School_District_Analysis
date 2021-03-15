# School_District_Analysis
_Analysis of School District Data with 'Jupyter Notebook','Anaconda','Python' & 'Pandas'_
---
## _Overview of Project_
The goal of the School District Analysis project was to utilize Pandas' in 'Jupyter Notebook' to deliver multiple high-level insights, in table format, on the relative performances of the district's 15 schools. 

In order to complete this brief for Maria and her respective school board, the 'students_complete.csv' required further data cleaning and replacing, after the school board discovered evidence of altered data points, the math and reading standardized test scores for 9th graders at Thomas High School. 

###__Deliverable 1__

Deliverable 1 mandates the replacement of Thomas High School's 9th grade reading and math test scores with 'NaNs', while protecting the remaining contents of the 'DataFrame'.

The following tasks were completed in order to satisfy __Deliverable 1__ requirements:
- [x] The 'loc' method was used to
  - Select and extract the math and reading scores from 9th graders at Thomas High School wit
- [x] the '==' comparison operator was wrapped inside 'loc()' to retrieve:
  - all rows with ninth grade in "grade" column of 'student_data_df'at THS
  - all the rows with the "reading_score" column of student_data_df at THS
  - all the rows with the "math_score" column of the student_data_df at THS
 - [x] reading and math scores, for 9th graders at THS '=np.nan'
 
Deliverable 1: Cleaned DataFrame 'student_data_df'
![Deliverable_1_student_data_df.png](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Cleaned Code\Deliverable_1_student_data_df.png)

Deliberable 1: Code Block (Steps 1-4)
![Deliverable_1_code_block.png](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Cleaned Code\1.1_thru_1.4.png)

###__Deliverable 2__ 

Deliverable 2 progresses the school district analysis as it mandates that we repeat the necessary steps to update the code in 'PyCitySchools.ipynb', which will output the reinstated DataFrames in table format. 

The following required metrics are updated with the cleaned school district data in 'School_District_Analysis'

1) The district summary DataFrame
2) The school summary DataFrame
3) The top 5 performing schools, based on the overall passing percentage
4) The bottom 5 performing schools. based on the overall passing percentage
5) The average math score for each grade level from each school
6) The average reading score for each grade level from each school
7) The scores by school spending per student
8) THe scores by school size
9) The scores by school type
---
## Results

1) _'district_summary_df':_

![2_district_summary_df](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Cleaned Code\2_district_summary_df.png)

2) _'per_school_summary_df':_

![deliverable2_per_school_summary_NEW.png](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Cleaned Code\deliverable2_per_school_summary_NEW.png)

3) _'top_performing_schools.head()':_

![top_schools_NEW.png](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Cleaned Code\top_schools_NEW.png)

4)_'bottom_performing_schools.head()':_

![bottom_schools_NEW.png](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Cleaned Code\bottom_schools_NEW.png)

5) _'avg_math_score_by_grade':_

![avg_math_grade_NEW.png](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Cleaned Code\avg_math_grade_NEW.png)

6) _'avg_reading_score_by_grade':_

![avg_read_grade_NEW.png](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Cleaned Code\avg_read_grade_NEW.png)

7) _'spending_summary_df':_

![spending_summary_NEW.png](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Cleaned Code\spending_summary_NEW.png)

8) _'size_summary_df':_

![size_summary_NEW.png](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Cleaned Code\size_summary_NEW.png)

9) _'type_summary_df':_

![type_summary_NEW.png](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Cleaned Code\type_summary_NEW.png)
---
### Deliverable 2 Findings : Effects on DataFrame Cleanup on 'PyCitySchools_Challenge.ipynb'

The below analyses list the effects of cleaning the data (replacing ninth-grade scores with NaNs) on each key metric 'DataFrame':

#### District Summary

__Before 'school_data_df' Cleanup__
- Average Math Score : 79.0
- Average Reading Score : 81.9
- % Passing Math : 75
- % Passing Reading : 86
- % Overall Passing : 65

__PyCitySchools file__
![district_summary_df_OLD.png](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Old Code\district_summary_df_OLD.png)

__Ater 'school_data_df' Cleanup__
- Average Math Score : 78.9
- Average Reading Score : 81.9
- % Passing Math : 74.8
- % Passing Reading : 85.7
- % Overall Passing : 64.9

__PyCitySchools_Challege file__
![district_summary_df_NEW.png](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Cleaned Code\district_summary_df_NEW.png)


#### School Summary (per_school_summary_df)

__Before 'school_data_df' Cleanup__

__PyCitySchools file__
![_per_school_summary_OLD.png](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Old Code\_per_school_summary_OLD.png)

__Ater 'school_data_df' Cleanup__
- Average Math Score : 78.9
- Average Reading Score : 81.9
- % Passing Math : 74.8
- % Passing Reading : 85.7
- % Overall Passing : 64.9

#### Thomas High School Relative Performance (9th grade math and reading scores = NaNs)

Repalcing the ninth graders' math and reading scores for Thomas High School changed THS relative ranking compared to other schools' performances.

- Before cleanup: 2nd place 
- After cleanup: 8th place

#### *per_school_summary_df*

__PyCitySchools file__
![per_school_summary_df_tail_OLD.png](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Old Code\per_school_summary_df_tail_OLD.png)

__PyCitySchools_Challege file__
![per_school_summary_THS_new](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Cleaned Code\per_school_summary_THS_new.png)

#### *top_performing_schools*

__PyCitySchools file__
![top_schools_OLD.png](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Old Code\top_schools_OLD.png)

__PyCitySchools_Challenge file__
![top_schools_NEW.png](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Cleaned Code\top_schools_NEW.png)

##### Math and Reading Scores By Grade

__Before Cleanup__

__PyCitySchools file__
![math_read_grade_OLD.png](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Old Code\math_read_grade_OLD.png)

__After Cleanup__

__PyCitySchools_Challege file__
![math_read_grade.NEW.png](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Cleaned Code\math_read_grade_NEW.png)

##### Scores by School Spending 

__Before Cleanup__

__PyCitySchools file__
![spending_summary_OLD.png](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Old Code\spending_summary_OLD.png)

__After Cleanup__

__PyCitySchools_Challege file__
![spending_summary_NEW.png](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Cleaned Code\spending_summary_NEW.png)

##### Scores by School Size

__Before Cleanup__

__PyCitySchools file__
![size_summary_OLD.png](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Old Code\size_summary_OLD.png)

__After Cleanup__

__PyCitySchools_Challege file__
![size_summary_NEW.png](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Cleaned Code\size_summary_NEW.png)

##### Scores by School Type

__Before Cleanup__

__PyCitySchools file__
![type_summary_OLD.png](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Old Code\type_summary_OLD.png)

__After Cleanup__

__PyCitySchools_Challege file__
![type_summary_NEW.png](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Cleaned Code\type_summary_NEW.png)
---
### Summary
__Major Changes in Updated School District Analysis:__
*After reading/math scores for ninth graders at Thomas High School = NaNs*

1) THS with removed 9th grade scores (NaNs treated as "=0") reduces the school's:
  - % Passing Math
  - % Passing Reading
  - % Overall Passing
2) Thomas High School's nullified 9th grade data, *greatly* affected the school's "% Overall Passing"
  - student_count before cleanup:1635
  - student_count after cleanup: 1174
  - % Overall Passing decrease by 25 ppts (from 90% to 60%)
  
Removing the ~500 9th graders purposely inflated grades brings the school's average down significantly, with only 10th-12th grade averages being weighted along with the school_count of 10th-12th grade students only.

3) Spending bin "$630-644", has reduced (lower) performance metrics:
  - % Passing Math
  - % Passing Reading
  - % Overall Passing
    - THS is allocated to spending bucket "$630-644
   
4) Thomas High School per school summary average math and reading scores are more inelastic than % passing math and passing reading
  - Average reading and math score by grade did not vary much
  - All grades had average math and reading scores around 80%, so when we remove the 9th grade scores from these averages:
    -The new average scores are barely changed as the score distrubtions between each grade is relatively constant
  - If school performance was reflective of average math and reading scores (weighted average), THS relative ranking would not have been chaned much either
