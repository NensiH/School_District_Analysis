# School_District_Analysis
The purpose of this project is to analyze the data of an entire School District, such as funding and student grades, to learn new insights and visually provide clear results on each school's performance and to find the overall passing percentages of the students and see if there is any correlation with the budget per student. 
[schools_complete.csv](https://github.com/NensiH/School_District_Analysis/files/7534912/schools_complete.csv)
 shows evidence of reading and math grades for Thomas High School ninth graders appears to have been altered. Since these values are missing we want to take all of the scores from the high school so that it doesn't affect our overall numbers. The analysis conducted compares previous school district analysis against this firm's analysis in order to determine how the suspected academic dishonesty affects school performance.

The school board has requested the following deliverables:

- A high-level District's summary 
- An overview of the each school
- Tables presenting each of the following metrics:
  - Based on the overall passing rate, Top 5 and bottom 5 performing schools
  - The average math score of students in each grade level at each school
  - The average reading score of students in each grade level at each school
  - School performance based on the budget per student
  - School performance based on the school size
  - School performance based on the type of school

## Development Environment
* Software: Python 3.7, Anaconda, Jupyter Notebook( numpy & panda lib)

## Resources
 [schools_complete.csv](https://github.com/NensiH/School_District_Analysis/files/7534914/schools_complete.csv)
 
 [students_complete.csv](https://github.com/NensiH/School_District_Analysis/files/7534915/students_complete.csv)


 
## Results
### District Summary
After taking a look at both district summaries from pycityschools and pycityschools_challenge there is a minor change.
The entire ninth grade class of Thomas High School have had their scores replaced with NaN. The DataFrame below is a summary representing the District after replacing the ninth graders' scores with NaN.

<img width="955" alt="Screen Shot 2021-11-14 at 4 04 16 PM" src="https://user-images.githubusercontent.com/92277581/141700408-77c8c7b1-f438-40d6-b75e-1969b5b2ed40.png">

### School Summary

The over all passing for Thomas High School was 90.94% in pycityschools, with the 9th graders taken out the overall passing shrinks by 0.3 %.
<img width="903" alt="Screen Shot 2021-11-14 at 4 07 02 PM" src="https://user-images.githubusercontent.com/92277581/141700484-3dac1a95-f56c-4b26-b915-e0da828764c1.png">

### Thomas High School Scores

Math and reading scores for ninth graders at Thomas High School were replaced with 'NaN' (null) so that their scores would not affect future calculations. If all of the students' scores were replaced with a 'O', then this would negatively impact averages for the school and school district. Overall it does not affect either the reading scores or math scores.

#### Thomas High School math scores:
Ninth grade math scores were replaced with 'NaN'. Thomas High School 10th, 11th, and 12th grade math scores are as follows: 83.1, 83.5, and 83.5.

<img width="271" alt="Screen Shot 2021-11-14 at 4 20 24 PM" src="https://user-images.githubusercontent.com/92277581/141701012-fb8da4a1-0528-4211-97d6-90b847af26ec.png">

#### **Thomas High School reading scores:**
Ninth grade math scores were replaced with 'NaN'. Thomas High School 10th, 11th, and 12th grade reading scores are as follows: 84.3, 83.6, and 83.8.

<img width="279" alt="Screen Shot 2021-11-14 at 4 28 14 PM" src="https://user-images.githubusercontent.com/92277581/141701095-9fd4e2a7-e840-4f09-a54a-f27b1b1c5364.png">

### Scores by School Spending
District spending per school was calculated by determining average spending ($620), standard deviation (~30), minimum spending amount ($578), lower quartile ($592), mid quartile ($628), upper quartile ($642), and mximum spending amount ($655) across all 15 schools:


<img width="243" alt="Screen Shot 2021-11-14 at 4 32 06 PM" src="https://user-images.githubusercontent.com/92277581/141701216-edbc24f6-9c6d-4b16-b85e-b6e0deeb7bf1.png">
Based on the figures given by the .describe() method, spending ranges per student in the school district were determined: $0-584, $585-629, $630-644, $645-675


<img width="489" alt="Screen Shot 2021-11-14 at 4 34 57 PM" src="https://user-images.githubusercontent.com/92277581/141701314-3d1ba732-6716-4e25-a98d-44b788da018c.png">


<img width="782" alt="Screen Shot 2021-11-14 at 4 46 30 PM" src="https://user-images.githubusercontent.com/92277581/141701744-6f7a2df6-1286-49d7-a582-55c4f11944f2.png">
It is found that Average Scores and Passing Percentages do not increase as spending per student increases.

### Scores by School Size
Scores by school size were calculated by determining size ranges for all 15 schools in the district: Small (<1000) Medium (1000-2000) Large (2000-5000)

As per my analysis, When considering School Sizes, "Large" Schools (Over 2,000 Students) have the lowest average scores and passing percentages. Small- and medium-sized schools in this district are very close in performance.

<img width="722" alt="Screen Shot 2021-11-14 at 4 54 49 PM" src="https://user-images.githubusercontent.com/92277581/141701970-6b840bb8-47b2-452c-b291-239448fc7c2a.png">

### Scores by School Type
Charter schools generally performed better than District schools in this analysis. The top five schools with the highest overall passing percentages are all Charter schools, whereas the bottom five are all District Schools. As seen in the DataFrame below, Charter schools have a 36% higher overall passing percentage than District schools.


<img width="727" alt="Screen Shot 2021-11-14 at 4 59 00 PM" src="https://user-images.githubusercontent.com/92277581/141702123-a7a91279-968b-448b-82d2-5b05434d83a2.png">

### Average Scores by Grade Level
After analyzing the average scores for math and reading by grade level for each school, it is found that a students grade level does not affect their scores as much as the school that they attend. The average scores within each school only varries by 1-2% depending on grade level. However, the difference in scores is more apparent when comparing different schools.

## Summary

Removing 9th grade student scores from Thomas High School affected the school district in the following ways:

- Average math scores dropped slightly (<1%)
- Average reading scores were not affected
- Percentage of students passing math dropped slightly (-1%)
- Percentage of students passing reading dropped slightle (-1%)
- The overall passing rate dropped (-1%)


Only scores for Thomas High School were affected:

- Perentage of students passing math dropped from 93.2% to 66.9%
- Percentage of students passing reading dropped from 97.3% to 69.7%
- Overall passing percentage dropped from 90.9% to 65.1%


Thomas High school is in the top 5 high school's list.

After we have replaced the scores of the 9th grade students we learn that not much has changed. We have nullified the values that we felt would alter size, district, spending and overall passing percentage of the students.



