# School_District_Analysis
## Overview of the school district analysis
 The main purpose of this analysis is to analyize the data of an entire school district,to verify state-testing standards, this analysis was conduced twice due to potential academic dishonesty among a group of students. . The school board has the students_complete.csv file shows evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered.Although the school board does not know the full extent of the academic dishonesty, they want to uphold state-testing standards. They want to replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. Once we have replaced the math and reading scores, then repeat the school district analysis that we did in this module and write up a report to describe how these changes affected the overall analysis.
 
Here is the list of deliverables for the analysis of the school district:

 1. A high-level snapshot of the district's key metrics, presented in a table format.
 
 2. An overview of the key metrics for each school, presented in a table format
 
 3. Tables presenting each of the following metrics:
 
    Top 5 and bottom 5 performing schools, based on the overall passing rate.
    
    The average math score received by students in each grade level at each school.
    
    The average reading score received by students in each grade level at each school.
    
    School performance based on the budget per student.
    
    School performance based on the school size.
    
    School performance based on the type of school.
  
## Resources

1. Data Source: PyCitySchools.ipynb file

2. Software: Python, Visual Studio Code, Anaconda, Jupyter Notebook, Pandas


## Results

### District summary 

The below dataframe represents the summary of the Thomas High School after replacing the nineth graders score with NaN.After relpacing the nineth graders math and reading scores by NaN, results the following changes in Thomas High School:

   1.The overall passing percentage for the entire district fell to 64.9%.
   
   2.The average math score droppped by .1%.
   
   3.The overall passing for reading scores dropped by .1%.
   
   4.The overall passing for math dropped by .2%.
   
![district summary](https://github.com/akthersr/School_District_Analysis/blob/main/Resources/district%20summary.png)

## School summary

The below figure shows the bottom five schools based on the overall passing rate.

![](https://github.com/akthersr/School_District_Analysis/blob/main/overall%20passing%20of%20bottom%20school.png)



