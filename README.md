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
<img src="https://github.com/sparrishmatt/School_District_Analysis/blob/main/Resources/9thnan.png" width="500">

#### District summary after grade removal
<img src="https://github.com/sparrishmatt/School_District_Analysis/blob/main/Resources/districtsummary.png" width="800">
