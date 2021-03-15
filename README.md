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

### Deliverable 2 Findings : Effects on DataFrames in 'PyCitySchools_Challenge.ipynb'

