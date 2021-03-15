# School_District_Analysis
_Analysis of School District Data with `Jupyter Notebook`, `Anaconda`,`Python` & `Pandas`
---
## Overview of Project
The goal of the School District Analysis project was to utilize `Pandas` in `Jupyter Notebook` to deliver multiple high-level insights, in table format, on the relative performances of the district's 15 schools. 

In order to complete this brief for Maria and the respective school board, the `students_complete.csv` required further data cleaning and replacing, after the school board discovered evidence of altered data points, the math and reading standardized test scores for 9th graders at Thomas High School. 

### Deliverable 1
Deliverable 1 mandates the replacement of Thomas High School's 9th grade reading and math test scores with `NaNs`, while protecting the remaining contents of the `DataFrame`.

The following tasks were completed in order to satisfy __Deliverable 1__ requirements:
- [x] The `loc` method was used to
  - Select and extract the math and reading scores from 9th graders at Thomas High School wit
- [x] the `==` comparison operator was wrapped inside `loc()` to retrieve:
  - all rows with ninth grade in "grade" column of `student_data_df'at THS
  - all the rows with the "reading_score" column of `student_data_df` at THS
  - all the rows with the "math_score" column of the `student_data_df` at THS
 - [x] reading and math scores, for 9th graders at THS `=np.nan`
 
Deliverable 1: Cleaned DataFrame `student_data_df`
<img width="699" alt="Deliverable_1_student_data_df" src="https://user-images.githubusercontent.com/77628698/111105493-79e2eb80-8529-11eb-931d-608be590727a.png">


Deliverable 1: Code Block (Steps 1-4)
<img width="831" alt="Deliverable_1_code_block" src="https://user-images.githubusercontent.com/77628698/111105630-cc240c80-8529-11eb-8a5e-6af6b68a7962.png">

### Deliverable 2
Deliverable 2 mandates that we repeat the necessary steps to update the code in 'PyCitySchools.ipynb', which will output the reinstated DataFrames in table format. 

The following required metrics are updated with the cleaned school district data in `School_District_Analysis`

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

1) _`district_summary_df`:_

<img width="826" alt="2_district_summary_df" src="https://user-images.githubusercontent.com/77628698/111105553-a26ae580-8529-11eb-8678-99981807ac92.png">


2) _`per_school_summary_df`:_

<img width="818" alt="deliverable2_per_school_summary_NEW" src="https://user-images.githubusercontent.com/77628698/111105575-b1519800-8529-11eb-9707-23a6207079a7.png">


3) _`top_performing_schools.head()`:_
<img width="822" alt="top_schools_NEW" src="https://user-images.githubusercontent.com/77628698/111105692-e4942700-8529-11eb-9f5d-2a7ed0ff0d58.png">

4)_`bottom_performing_schools.head()`:_
<img width="829" alt="bottom_schools_NEW" src="https://user-images.githubusercontent.com/77628698/111105703-ea8a0800-8529-11eb-9cbd-8e760ff04330.png">

5) _`avg_math_score_by_grade`:_
<img width="409" alt="avg_math_grade_NEW" src="https://user-images.githubusercontent.com/77628698/111105707-eeb62580-8529-11eb-98a5-63fec9460749.png">

6) _`avg_reading_score_by_grade`:_
<img width="405" alt="avg_read_grade_NEW" src="https://user-images.githubusercontent.com/77628698/111105749-01305f00-852a-11eb-93da-fb609decf595.png">

7) _`spending_summary_df`:_

<img width="769" alt="spending_summary_NEW" src="https://user-images.githubusercontent.com/77628698/111105767-0d1c2100-852a-11eb-9dd7-d4c0e3c8747b.png">


8) _`size_summary_df`:_

<img width="823" alt="size_summary_NEW" src="https://user-images.githubusercontent.com/77628698/111105777-14dbc580-852a-11eb-9524-fe4a0fbebed6.png">

9) _`type_summary_df`:_
<img width="836" alt="type_summary_NEW" src="https://user-images.githubusercontent.com/77628698/111105844-38067500-852a-11eb-8309-5b5c5ddc236c.png">

---
### Deliverable 2 Findings : Effects on DataFrame Cleanup on `PyCitySchools_Challenge.ipynb`

The below analyses list the effects of cleaning the data (replacing ninth-grade scores with NaNs) on each key metric `DataFrame`:

#### District Summary

__Before `school_data_df Cleanup__
- Average Math Score : 79.0
- Average Reading Score : 81.9
- % Passing Math : 75
- % Passing Reading : 86
- % Overall Passing : 65

__PyCitySchools file__
<img width="818" alt="district_summary_df_OLD" src="https://user-images.githubusercontent.com/77628698/111105878-53718000-852a-11eb-84a3-e63e736ed402.png">

__Ater 'school_data_df' Cleanup__
- Average Math Score : 78.9
- Average Reading Score : 81.9
- % Passing Math : 74.8
- % Passing Reading : 85.7
- % Overall Passing : 64.9

__PyCitySchools_Challege file__
<img width="775" alt="district_summary_df_NEW" src="https://user-images.githubusercontent.com/77628698/111105901-6a17d700-852a-11eb-8a94-2886e15a051a.png">

#### School Summary (per_school_summary_df)

__Before `school_data_df` Cleanup__

__PyCitySchools file__
<img width="815" alt="per_school_summary_df_OLD" src="https://user-images.githubusercontent.com/77628698/111105937-7a2fb680-852a-11eb-965d-eedc53ef0a54.png">

__After `school_data_df` Cleanup__

__PyCitySchools_Challenge file__
<img width="818" alt="deliverable2_per_school_summary_NEW" src="https://user-images.githubusercontent.com/77628698/111105958-8451b500-852a-11eb-8f2f-b29df58d1010.png">

#### Thomas High School Relative Performance (9th grade math and reading scores = NaNs)

Repalcing the ninth graders' math and reading scores for Thomas High School changed THS relative ranking compared to other schools' performances.

- Before cleanup: 2nd place 
- After cleanup: 8th place

#### `per_school_summary_df`

__PyCitySchools file__
<img width="830" alt="per_school_summary_df_tail_OLD" src="https://user-images.githubusercontent.com/77628698/111105989-929fd100-852a-11eb-80bc-7f913785cb8a.png">

__PyCitySchools_Challege file__
<img width="804" alt="per_school_summary_THS_new" src="https://user-images.githubusercontent.com/77628698/111105997-97648500-852a-11eb-8590-d70aff3877e8.png">

#### `top_performing_schools`

__PyCitySchools file__
<img width="836" alt="top_schools_OLD" src="https://user-images.githubusercontent.com/77628698/111106013-9fbcc000-852a-11eb-8ceb-9133ae09fdfb.png">

__PyCitySchools_Challenge file__
<img width="822" alt="top_schools_NEW" src="https://user-images.githubusercontent.com/77628698/111106021-a5b2a100-852a-11eb-957f-becab22b0c6d.png">

##### Math and Reading Scores By Grade

__Before Cleanup__

__PyCitySchools file__
<img width="396" alt="math_read_grade_OLD" src="https://user-images.githubusercontent.com/77628698/111106033-acd9af00-852a-11eb-88ef-29e1c954b5f9.png">

__After Cleanup__

__PyCitySchools_Challege file__
<img width="370" alt="math_read_grade_NEW" src="https://user-images.githubusercontent.com/77628698/111106042-b236f980-852a-11eb-8967-df1adc48548f.png">

##### Scores by School Spending 

__Before Cleanup__

__PyCitySchools file__
<img width="707" alt="spending_summary_OLD" src="https://user-images.githubusercontent.com/77628698/111106099-ce3a9b00-852a-11eb-90b7-7a5e2b04541b.png">

__After Cleanup__

__PyCitySchools_Challege file__
<img width="769" alt="spending_summary_NEW" src="https://user-images.githubusercontent.com/77628698/111106121-d561a900-852a-11eb-9e8e-a05c1baea3bc.png">


##### Scores by School Size

__Before Cleanup__

__PyCitySchools file__
<img width="707" alt="size_summary_OLD" src="https://user-images.githubusercontent.com/77628698/111106138-dabef380-852a-11eb-9b48-e67e21482349.png">


__After Cleanup__

__PyCitySchools_Challege file__
<img width="823" alt="size_summary_NEW" src="https://user-images.githubusercontent.com/77628698/111106152-e0b4d480-852a-11eb-855e-e54b8386a7dd.png">

##### Scores by School Type

__Before Cleanup__

__PyCitySchools file__
<img width="646" alt="type_summary_OLD" src="https://user-images.githubusercontent.com/77628698/111106164-e8747900-852a-11eb-9265-1b6bb3d2afa9.png">


__After Cleanup__

__PyCitySchools_Challege file__
<img width="836" alt="type_summary_NEW" src="https://user-images.githubusercontent.com/77628698/111106170-ec080000-852a-11eb-8763-5b105a903f86.png">

---
### Summary
__Major Changes in Updated School District Analysis:__
*After reading/math scores for ninth graders at Thomas High School = NaNs*

1) THS with removed 9th grade scores (NaNs treated as "=0") reduces the school's:
  - % Passing Math
  - % Passing Reading
  - % Overall Passing
2) Thomas High School's nullified 9th grade data, __*greatly*__ affected the school's "% Overall Passing"
  - student_count before cleanup:1635
  - student_count after cleanup:1174
  - % Overall Passing decrease by 25 ppts (from 90% to 60%)
  
Removing the ~500 9th graders' incorrect and inflated grades:
- brings the school's total amount of students who passed both math and reading (10th-12th only) down greatly.

3) Spending bin "$630-644", has reduced (lower) performance metrics:
  - % Passing Math
  - % Passing Reading
  - % Overall Passing
    - THS is allocated to spending bucket "$630-644
   
4) Thomas High School per school summary average math and reading scores are more inelastic than % passing math and passing reading
  - Average reading and math score by grade did not vary much
  - All grades had average math and reading scores around 80%, so when we remove the 9th grade scores from these averages:
    - The new average scores are barely changed as the score distrubtions between each grade is relatively constant
  - If school performance was reflective of average math and reading scores (weighted average):
    - THS relative ranking would not have been chaned much either
