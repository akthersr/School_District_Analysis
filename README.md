# School_District_Analysis
## Overview of the school district analysis
 The main objective of this analysis is to analyize the data of an entire school district,such as school funding,school size,student grades and the standrized state test scores for math and reading of each students in the district,to learn new insights and provide visual results on each schools performance.
 
 The school board has notified the chief data scientist for a school district, Maria and her supervisor that the students_complete.csv file shows evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. Although the school board does not know the full extent of the academic dishonesty, they want to to verify state-testing standards. They want to replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact.Additionally, to uphold state-testing standards, this analysis was conduced twice due to potential academic dishonesty among a group of students.
 
## Purpose of the analysis

The main purpose of this analysis to analyze the state-testing score for math test and reading test from nineth to twelfth grade in different high schools of the district. Here is the list of deliverables for the analysis of the school district:

 1. A high-level snapshot of the district's key metrics, presented in a table format.
 2. An overview of the key metrics for each school, presented in a table format.
 3. Tables presenting each of the following metrics:
 
    The district summary.
    The school summary.
    Top 5 and bottom 5 performing schools, based on the overall passing rate.
    The average math score received by students in each grade level at each school.
    The average reading score received by students in each grade level at each school.
    School performance based on the budget per student.
    School performance based on the school size.
    School performance based on the type of school.
  
## Resources

1. Data Source:students_complete.csv,schools_complete.csv.
2. Software: Python, Visual Studio Code, Anaconda, Jupyter Notebook, Pandas.
3. Output Files: PyCitySchools.ipynb & PyCitySchools_Challenge.ipynb 

## Analysis

### Replace the reading and math scores


With the help of Numpy and Pandas libraries, we read the two csv files on School Data and Student Data. At first,using the loc method on the student dataframe we replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact.

![](https://github.com/akthersr/School_District_Analysis/blob/main/9th%20grade%20nan.png)

The below figure shows the student dataframe:

![](https://github.com/akthersr/School_District_Analysis/blob/main/student%20data%20frame%20nan.png)

 ### Repeat the school district analysis
 
 The two dataframe were merge together for further analysis.Then,we have to recalculate the total student count by subtracting the number of ninth-grade students in Thomas High School(THS) from the total student count, recalculate the passing math and passing reading percentages, and the overall passing percentage with the recalculated total student count.
 
 ![](https://github.com/akthersr/School_District_Analysis/blob/main/ths%20count.png)
 
 A school summary dataframe was created to update the school summary using the 10th-12th graders from Thomas High School(THS).For this,we have to calculate the total number of students from 10th to 12th grade in Thomas High School.
 
From this dataset we create three new DataFrames for the 10th-12th graders from Thomas High School: passing math rate,  passing reading rate, and overall passing rate for both math and reading.

![](https://github.com/akthersr/School_District_Analysis/blob/main/overall%20ths.png)

We replace the % Passing Math, % Passing Reading, and % Overall Passing scores in the current School Summary DataFrame with the new passing percentages for Thomas High School. Top and bottom five performing schools were determined by sorting the school summary dataframe on overall passing rate.Next, the performance of school scores were analyzed by school budget per student and  school size.At the end, we determine the performace of schools by school type.
 
 ## Results

### District summary 

The DataFrame below shows the District summary with the full set of student data.

![](https://github.com/akthersr/School_District_Analysis/blob/main/district%20summary%20original.png)

The DataFrame below is a summary representing the District after replacing the ninth graders' scores with NaN.

![district summary](https://github.com/akthersr/School_District_Analysis/blob/main/Resources/district%20summary.png)

The change of adding Nan for grade 9 in Thomas High School math and reading scores did not have a large impact on the district analysis, with each metric decresing by less that 0.2 percentage point each (meaning scores changed by less than 0.5%). It's important to consider there are only 461 students in grade 9 at Thomas High School, and given the total student count is 39,170.The overall passing percentage for the entire district fell to 64.9%.
   
## School summary

In the original analysis, Thomas High School overall passing rate was 91%.But, after adjusting data for 9th graders had a very significant affect in THS test scores.The overall passing rate drop to 65%, passing rate in math was almost 67% and passing rate in reading 70%.

Original school summary:

![](https://github.com/akthersr/School_District_Analysis/blob/main/school%20summary%20THS.png)

School summary excluding 9th grader:

![](https://github.com/akthersr/School_District_Analysis/blob/main/school%20summary%20original.png)

The below figure shows the top five schools based on the overall passing rate.

![](

The below figure shows the bottom five schools based on the overall passing rate.

![](

The ranking of the top schools including Thomas High School was not affected by the update.While the average math, reading and overall scores at Thomas High School were impacted with the update, the changes were not enough to change its relative ranking versus other schools.



