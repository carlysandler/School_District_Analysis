# School_District_Analysis
Analysis of School District Data using 'Jupyter Notebook', 'Anaconda', 'Python' & 'Pandas' library
---

## _Overview of Project_
The goal of the School District Analysis project was to utilize Pandas' in 'Jupyter Notebook' to deliver multiple high-level insights, in table format, on the relative performances of the district's 15 schools. 

In order to complete this brief for Maria and her respective school board, the 'students_complete.csv' required further data cleaning and replacing, after the school board discovered evidence of altered data points, the math and reading standardized test scores for 9th graders at Thomas High School. 

__Deliverable 1__ thus mandates the replacement of Thomas High School's 9th grade reading and math test scores with 'NaNs', while protecting the remaining contents of the 'DataFrame'.

The following tasks were completed in order to satisfy __Deliverable 1__ requirements:
- [x] The 'loc' method was used to
  - Select and extract the math and reading scores from 9th graders at Thomas High School wit
- [x] the '==' comparison operator was wrapped inside 'loc()' to retrieve:
  - all rows with ninth grade in "grade" column of 'student_data_df'at THS
  - all the rows with the "reading_score" column of student_data_df at THS
  - all the rows with the "math_score" column of the student_data_df at THS
 - [x] reading and math scores, for 9th graders at THS '=np.nan'
 
Once these actions were taken and we ran the code in 'Jupyter Notebook'
Key metrics measuring relative school performance included:
-
- 
- metrics erformance varying school performance key metrics intra district school  for our clients, Maria and her respective district school board,
