#**School DISTRICT ANALYSIS**
##**Overview of the school district analysis: 

## **Explain the purpose of this analysis**
The school board has notified that the students_complete.csv file shows evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. Although the school board does not know the full extent of the academic dishonesty, they want to uphold state-testing standards.

So, the analysis involves  replacing the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. Once the math and reading scores those have been replaced, the school district analysis needs to be completed and describe how these changes affected the overall analysis.

# Resources
- File Source: schools_complete.csv
- File Source: students_complete.csv
- Software: Jupyter Notebook 6.4.8
- Library: Pandas
- Library: Numpy
- Language: Python 3.7.13

# **Results**

## How is the district summary affected?
Comparing the two summaries below, it is obvious that there was not much of an impact by removing the 9th graders from Thomas High School, by replacing their scores with NaN.  We have to keep in mind that there were only 461 students in the 9th grade at Thomas High School who were only 1.2% of the school population and the impact was almost less than 0.5% change in each of the metrics.

- The Average Math Score decreased from 79.0 to 78.9
- There was no change in the Average Reading Score, cruised at 81.8
- The % Passing Math decreased from 75.0% to 74.8%
- The % Passing Reading decreased from 85.8% to 85.7%
- The % Overall Passing decreased from 65.2% to 64.9%

![Original District Symmary](https://github.com/veenapu/School_District_Analysis/blob/main/Resources/Original%20District%20Summary.png)

![Updated District Summary](https://github.com/veenapu/School_District_Analysis/blob/main/Resources/Updated%20District%20Summary.png)

## How is the school summary affected?
Looking at Thomas High School for example in the screenshots below, there was an overall decrease or no change in the metrics except for the Math Score.

- There was no change in the Average Reading Score
- The Average Math Score increased from 83.8 to 83.9
- The % Passing Math decreased from 93.3% to 93.2%
- The % Passing Reading decreased from 97.3% to 97.0%
- The % Overall Passing decreased from 90.9% to 90.6%

![Original Per School Summary](https://github.com/veenapu/School_District_Analysis/blob/main/Resources/Original%20Per%20School%20Summary.png)

![Updated Per School Summary](https://github.com/veenapu/School_District_Analysis/blob/main/Resources/Updated%20Per%20School%20Summary.png)


## How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
Thomas High School was 2nd position amongst all schools initially, based on the % Overall Passing Score of 90.9%. But, after replacing the scores for the ninth graders, Thomas High School dropped to 3rd position with the % Overall Passing Score of 90.6% 

The bottom schools were not affected at all, as Thomas High School was not in the bottom five.

- There was no change in the Average Reading Score, remained at 83.4 
- The Average Math Score increased from 83.8 to 83.9
- The % Passing Math decreased from 93.3% to 93.2%
- The % Passing Reading decreased from 97.3% to 97.0%
- The % Overall Passing decreased from 90.9% to 90.6%

![Original Top 5 schools](https://github.com/veenapu/School_District_Analysis/blob/main/Resources/Original%20Top%205%20Schools.png)

![Updated Top 5 schools](https://github.com/veenapu/School_District_Analysis/blob/main/Resources/Updated%20Top%205%20Schools.png)

![Original Bottom 5 schools](https://github.com/veenapu/School_District_Analysis/blob/main/Resources/Original%20Bottom%205%20Schools.png)

![Updated Bottom 5 schools](https://github.com/veenapu/School_District_Analysis/blob/main/Resources/Updated%20Bottom%205%20Schools.png)


## How does replacing the ninth-grade scores affect the following:
## Math and reading scores by grade
Thomas High School has Nan for 9th grade for both Math and Reading Scores.  Therefore, calculating the average would be more meaningful.

Average 9th grade Reading Scores decreased from 82.5 to 82.4 after Thomas High School 9th graders were excluded. 

Average 9th grade Math Scores decreased from 80.4 to 80.1 after Thomas High School 9th graders were excluded.

![Original Math Scores by Grade](https://github.com/veenapu/School_District_Analysis/blob/main/Resources/Original%20Math%20Scores%20by%20Grade.png)

![Updated Math Scores by Grade](https://github.com/veenapu/School_District_Analysis/blob/main/Resources/Updated%20Math%20Scores%20by%20Grade.png)

![Original Reading Scores by Grade](https://github.com/veenapu/School_District_Analysis/blob/main/Resources/Original%20Reading%20Scores%20by%20Grade.png)

![Updated Reading Scores by Grade](https://github.com/veenapu/School_District_Analysis/blob/main/Resources/Updated%20Reading%20Scores%20by%20Grade.png)

## Scores by school spending
Thomas High School falls within the $630-$644 per capita spending bin. Within this bin, while the % Passing Reading decreased from 84.4% to 84.3%, and % Overall Passing decreased from 62.9% to 62.8%, a very small change; there was no change in the rest of the metrics.

![Original School Spending](https://github.com/veenapu/School_District_Analysis/blob/main/Resources/Original%20School%20Spending.png)

![Updated School Spending](https://github.com/veenapu/School_District_Analysis/blob/main/Resources/Updated%20School%20Spending.png)

## Scores by school size
Within this bin, while the % Passing Reading decreased from 96.8% to 96.7% and the % Overall Passing decreased from 90.6% to 90.5%; there was no change in the rest of the metrics. Thomas High Schools falls under the medium sized school bracket.

![Original Scores by School Size](https://github.com/veenapu/School_District_Analysis/blob/main/Resources/Original%20Scores%20by%20School%20Size.png)

![Updated Scores by School Size](https://github.com/veenapu/School_District_Analysis/blob/main/Resources/Updated%20Scores%20by%20School%20Size.png)

## Scores by school type
Within this bin, the % Passing Reading decreased from 96.6% to 96.5% while the rest of the metrics remained the same. 

![Original Scores by School Type](https://github.com/veenapu/School_District_Analysis/blob/main/Resources/Original%20Scores%20by%20School%20Type.png)

![Updated Scores by School Type](https://github.com/veenapu/School_District_Analysis/blob/main/Resources/Updated%20Scores%20by%20School%20Type.png)


# **Summary**
## Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

There are quite a few changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.  Here are four of them:

1.	Looking at the Scores by School Size, changes to Medium (1000-2000) grouping size was less than 0.1% for all metrics. Thomas High School falls under this bin.
2.	Looking at the Scores by School Type, changes to Charter type grouping was less than 0.1%, for all metrics.  Thomas High School is a charter school.
3.	Based on the District Summary, changes to all scores were changed by less than 0.5%, without any impact to school or student count.
4.	No changes to overall school ranking.  Thomas High School remained in the same position, however it’s scores did change by less than 1% for each the metrics.

