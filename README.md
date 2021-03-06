#### School_District_Analysis
### Overview
The purpose of this analysis was to remove the ninth grade students accused of cheating at Thomas High School from our dataset to see how this affected our results for both the school and district summaries. 

## Results
The district summary is affected in that there are now a smaller number of total students (due to removed ninth graders from Thomas High School). The metrics for Average Reading/Math Score, and passing percentages for reading, math, and overall were slightly changed, showing a small decrease across all categories. 

District Summary with Thomas 9th graders:
![with_ninth_graders](District_summary_ninth_graders.PNG)

District Summary without Thomas 9th graders:
![without_ninth_graders](District_summary_no_ninth_graders.PNG)

The results for Thomas High School are affected, with passing percentages for math, reading, and overall all falling (but only slightly). Removing the ninth graders from the dataset does not change the standing of THS relative to other schools in the district, as it still ranks second in terms of performance after removing the ninth grade students. 

Top Five Schools (After removal of THS 9th graders):
![top_five_schools](top_five_schools.png)


# Summary
Removing the ninth graders from Thomas High School from the dataset changes the results of our analysis by affecting:
1) The total number of students in the dataset
2) Average reading and math Scores for both THS and the district overall
3) Passing reading and math percentages for both THS and the district overall
4) Overall passing percentages fot both THS and the district overall

- It is important to note that we replaced the metrics for Thomas High School with the scores and percentages for their 10th-12th grade students, if we ran the analysis including the ninth grade students at THS with NaN values, their metrics in all categories would have dropped drastically (shown below), as about 1/4 of their students would be failing with scores of 0. 

Metrics for Thomas High School if we leave all 9th graders as Nan and don't replace with data for just 10th-12th grade students:
![with_NaN_values](if_ninth_graders_included_ths.png)
- This would result in drastic drops across metrics, especially in terms of passing percentages.
