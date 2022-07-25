# School District Analysis

## Analysis Overview
The purpose of this analysis is to examine the testing scores and passing percentages for all of the schools in a school district. An important point here is that the reading and math scores for Thomas High School might be illegitimate, so those scores must be removed to insure the best possible accuracy. Passing percentages will be found for all schools after these corrections are made, and then passing percentages based on school budget, school size, and school type (district or charter). 

## Removal of Scores
As was mentioned in the overview, the reading and math scores for 9th graders at Thomas High School must be removed. This was done by using the "loc" function to find those specific students and then setting their scores to NaN. An example score replacement can be seen here.

<img src="https://github.com/sparrishmatt/School_District_Analysis/blob/main/Resources/9thnan.png" width="500">

## Results of Analysis
### What effect on the results should we expect by removing the scores for the Thomas High School 9th graders?
* District Summary
By removing those scores it would be assumed that the average reading and writing scores for the district would drop. However, we should expect the drop to be small because the number of students being removed is not many compared to the number of students in the district.

#### District summary before grade removal
<img src="https://github.com/sparrishmatt/School_District_Analysis/blob/main/Resources/predistrictsummary.png" width="800">

#### District summary after grade removal
<img src="https://github.com/sparrishmatt/School_District_Analysis/blob/main/Resources/districtsummary.png" width="800">

This confirms that a very small percentage drop occurred for all percentage columns. It should also be noted that the average grade columns were not affected. The reasoning for this is that the average grades do not take the total number of grades or students into account, whereas the percent grade columns are dividing by the total number of students.

---

* School Summary

By looking at the percentage results for each school in the district instead of just the district results, we should expect the percentages for Thomas High School to be low for the same reasoning as above.

<img src="https://github.com/sparrishmatt/School_District_Analysis/blob/main/Resources/preperschoolsummary.png" width="800">

It would be unfair to have uncounted students affect the percentages of the school, so the student count for Thomas High School will be changed to only include grades 10-12 in the code for the percentage calculations. This will show the true percentages for grades 10-12. 

<img src="https://github.com/sparrishmatt/School_District_Analysis/blob/main/Resources/perschoolsummary.png" width="800">

As expected, the percentage results for Thomas High have been fixed and are now much higher. Thomas High School has now gone from having below average passing percentages to having some of the highest percentages of all schools. We can see this by looking at the top 5 schools ordered by their grades.

<img src="https://github.com/sparrishmatt/School_District_Analysis/blob/main/Resources/top5schools.png" width="800">


---

* Results by Grade


It should be expected that for both math and reading percentages, Thomas High School is listed as NaN for their 9th graders. 

* Scores by School Spending


Since this output was created after the count of 9th grade Thomas High students was removed from the total students, we can't see how Thomas High School's budget bracket is affected by the change, but compared to the output before the 9th graders had their scores changed to NaN there is not a big enough difference to change the results due to rounding. 

For the output itself, it is interesting to see that the grades and passing percentages are much higher for the lowest budget group. That seems like contrary to what would be expected, but the results are clear. 

* Scores by School Size

<img src="https://github.com/sparrishmatt/School_District_Analysis/blob/main/Resources/gradesbysize.png" width="800">

There is no notable difference in grades between small and medium schools, but large schools have much lower grades overall and much lower passing percentages. 

Once again, this is the same output as if the 9th graders had their scores included still. This can be interpreted as the 9th graders at Thomas High School scoring around the school averages for both math and reading. That would be the reason for the lack of changes and hence only one output has been included, which will continue for the next ouput.

* Scores by School Type

<img src="https://github.com/sparrishmatt/School_District_Analysis/blob/main/Resources/gradesbytype.png" width="800">

There is clearly a very notable difference in math and reading grades between district and charter schools, with charter schools having better percentages in every possible category. 

## School District Summary
From these results, it looks like medium sized charter schools are the best performing in this district. Thomas High School is included in this category, and clearly their scores are very high. There were some differences to the original outputs that were caused by removing the 9th graders from Thomas: the % passing reading, % passing math, and % overall passing were both affected by the removal, as well as those same percentages on a greater scale for Thomas High School. Because of those differences the code was changed to only include grades 10-12 for Thomas High School.



