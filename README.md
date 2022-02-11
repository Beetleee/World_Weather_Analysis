# Module 6  World Weather Analysis
### by Terra Lasho 

## Deliverable 1: Weather_Database folder with the following:
  ### The *Weather_Database.ipynb* file
  ### The WeatherPy_Database.csv file
  ### The Vacation_Search folder with the following:

The Vacation_Search.ipynb file
The WeatherPy_vacation.csv file
The WeatherPy_vacation_map.png image
The Vacation_Itinerary folder with the following:

The Vacation_Itinerary.ipynb file
The WeatherPy_travel_map.png image
The WeatherPy_travel_map_markers.png image
A README.md that describes the purpose of the repository. Although there is no graded written analysis for this challenge, it is encouraged and good practice to add a brief description of your project.
## Overview of the school district analysis: 
I am tasked to provide analysis on district reading and math grades for a school board.  There has been some evidence of nefarious activity with grades specifically in ninth grade at Thomas High School.  For this project, I need to first replace these grades with “NaN” (removing them from the data), and then perform district analysis on the other data.  In the end, we will compare the two datasets to see what is different. 

Explain the purpose of this analysis.
The purpose of this analysis is to view the difference in the data analysis after removal of a specific dataset.
## Deliverable 1/Code Setup and Specifics:
**Step1:** I first did a query (using .loc) to grab all 9th grade specific grades from Thomas High School (THS), and then replaced the 9th Grade THS scores with NaN (using .loc) and viewed the data

![](https://github.com/Beetleee/School_District_Analysis/blob/main/Resources/D1_Step1.png)

![](https://github.com/Beetleee/School_District_Analysis/blob/main/Resources/D1Step2_3.png)

**Step2:** Student count
-Number of Students in 9th Grade at THS:  **461**

-Total Student Count: **39,170**

-Remaining Number of Students after Removing 9th Grade at THS: **38,709**
	
![](https://github.com/Beetleee/School_District_Analysis/blob/main/Resources/specifics_on_9thTHS.png)


**Step3:** Math and Reading Percentages of New Student Count:

-Math passing percentages on New Student Count: **74.76%**

-Reading passing percentages on New Student Count: **85.66%**
	
![](https://github.com/Beetleee/School_District_Analysis/blob/main/Resources/percentages_on_new.png)

**Step4:** Overall Passing Percentage of New Student Count:

-Overall Passing Percentage: **64.86%**
	
![](https://github.com/Beetleee/School_District_Analysis/blob/main/Resources/overall.png)

**Step5:** Number of 10th – 12th grade students

-10th – 12th grade students: **1,174**
	
![](https://github.com/Beetleee/School_District_Analysis/blob/main/Resources/total10_12atTHS.png)

**Step6& 7:** Use .loc to create a df that has all students passing math and reading (separate) from THS

-Students (10th-12th from THS) passing math: **1,094**

-Students (10th-12th from THS) passing reading: **1,139**
	
![](https://github.com/Beetleee/School_District_Analysis/blob/main/Resources/10_12atTHS_passing.png)	

**Step8&9:** Use .loc to create a df with all students passing both math and reading from THS

-Students (10th-12th from THS) passing both math and reading: **1,064**
	
![](https://github.com/Beetleee/School_District_Analysis/blob/main/Resources/10_12atTHS_passingloc.png)

**Step10:** Calculate the percentage of 10th-12th graders passing reading from THS

-% Students (10th-12th at THS) passing reading percentage: **97.02%**
	
![](https://github.com/Beetleee/School_District_Analysis/blob/main/Resources/step10.png)

**Step11:** Calculate the overall passing percentage of 10th-12th graders from THS

-% Students (10th-12th at THS) overall passing percentage: **90.63%**
	
![](https://github.com/Beetleee/School_District_Analysis/blob/main/Resources/step11.png)

**Step12:** Use .loc to replace %passing math score for THS with new % calculated from Step 9

-% Students (10th-12th at THS) NEW math passing percentage: **93.19%** (no change)
	
![](https://github.com/Beetleee/School_District_Analysis/blob/main/Resources/step12.png)

**Step13:** Use .loc to replace %passing reading score for THS with new % calculated from Step 9

-% Students (10th-12th at THS) NEW reading passing percentage: **97.02%** (no change)
	
![](https://github.com/Beetleee/School_District_Analysis/blob/main/Resources/10_12atTHS_passing%reading.png)

**Step14:** Use .loc to replace %overall passing score for THS with new % calculated from Step 9

-% Students (10th-12th at THS) overall passing percentage: **90.63%**
	
![](https://github.com/Beetleee/School_District_Analysis/blob/main/Resources/10_12atTHS_passing%overall.png)

***Also provided in code output are several lists of deliverables:
-The Top and Bottom 5 schools (based on passing rate)
-Average math and reading score for each grade level from each school
-Scores by school spending per student, by school size, and by school type

## Results/Deliverable 2:

### How is the district summary affected?

-Removing ~500 9th grade scores from THS, gave a <1% difference.  

![](https://github.com/Beetleee/School_District_Analysis/blob/main/Resources/districtsummary.png)

### How is the school summary affected?

-THS had a 91% overall passing rate (which was concerningly high)..  After completing the 10th-12th grade student score analysis only, the testing was adjusted.

![](https://github.com/Beetleee/School_District_Analysis/blob/main/Resources/adjusted.png)	
**Results indicate that removing the 9th grade data had a big impact, by dropping the overall passing rate by 25%

![](https://github.com/Beetleee/School_District_Analysis/blob/main/Resources/bins.png)

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

-THS was #2 ranked in the top schools in the original analysis, but dropped to the middle of the pack after the new analysis 

![](https://github.com/Beetleee/School_District_Analysis/blob/main/Resources/location.png)

-In the original analysis, Thomas High School had 83.6 math average and 83.7 reading average for the 9th grade tests. Now the scores have been replaced with null values and new analysis is in the following charts:

#### Scores by school spending:

Thomas High School is in the $630-$644/student spending range. 

![](https://github.com/Beetleee/School_District_Analysis/blob/main/Resources/spending.png)

#### Scores by school size:

Thomas High School is defined as a medium sized school.

![](https://github.com/Beetleee/School_District_Analysis/blob/main/Resources/size.png)

#### Scores by school type:

There was very little impact by school type by changing the 9th grade scores. Thomas High School is a Charter type.

![](https://github.com/Beetleee/School_District_Analysis/blob/main/Resources/final.png)

## Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs. 

-The overall passing rate for Thomas High School was affected by removing 9th grade data from 91% to 65%.

-Thomas High School's ranking dropped from 2nd to 8th in the district, out of a total of 15 campuses.

-"NaN" is now in reports for the 9th grade students at Thomas High School

-Thomas High School’s math and reading averages and passing percentages all saw shifts.
