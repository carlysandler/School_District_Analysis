# School_District_Analysis
_Analysis of School District Data with 'Jupyter Notebook','Anaconda','Python' & 'Pandas'_
---

## _Overview of Project_
The goal of the School District Analysis project was to utilize Pandas' in 'Jupyter Notebook' to deliver multiple high-level insights, in table format, on the relative performances of the district's 15 schools. 

In order to complete this brief for Maria and her respective school board, the 'students_complete.csv' required further data cleaning and replacing, after the school board discovered evidence of altered data points, the math and reading standardized test scores for 9th graders at Thomas High School. 

__Deliverable 1__
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
![1.1_thru_1.4.png](C:\Users\carly\OneDrive\Desktop\data_bootcamp\analysis_projects\School_District_Analysis\Resources\Cleaned Code\1.1_thru_1.4.png)

__Deliverable 2__ 
Deliverable 2 progresses the school district analysis as it mandates that we repeat the necessary steps to update the code in 'PyCitySchools.ipynb', which will output the reinstated DataFrames in table format. 

The following required metrics are updated with the cleaned school district data in 'School_District_Analysis'

1) The district summary DataFrame
2) The school summary DataFrame
3) The top 5 performing schools, based on the overall passing percentage
4) The average math score for each grade level from each school
5) The average reading score for each grade level from each school
6) The scores by school spending per student
7) THe scores by school size
8) The scores by school type


Once these actions were taken and we ran the code in 'Jupyter Notebook'
Key metrics measuring relative school performance included:
-
- 
- metrics erformance varying school performance key metrics intra district school  for our clients, Maria and her respective district school board,
