# School District Analysis with PANDAS

## Overview of Project

### Background

After a specific school district analysis was run information was shared about potential academic dishonesty at one of the schools – Thomas High School (THS).  Specific grades were changed to NaN and the analysis was rerun to uphold state-testing standards

### Purpose

Starter code was provided to kick off the analysis.  The 9th grade math and reading scores at THS were changed to NaN utilizing the.loc() function and the entire analysis was rerun leveraging the starter code provided and the revised student data frame.

## Analysis Results

1.	How is the district summary affected?

-	The change was minimal in the school district summary with the 9th grade scores from THS removed.  All scores and percentages of passing changed by approximately a tenth of a percentage point.

Original District Summary:


![original_district_summary](https://user-images.githubusercontent.com/80165223/115123529-0cd8d080-9f83-11eb-9f5d-5ef1a59541ad.png)



Revised District Summary:


![revised_district_summary](https://user-images.githubusercontent.com/80165223/115123534-182bfc00-9f83-11eb-9ed2-2a30800caffa.png)



2.	How is the school summary affected?

-	While there were minimal changes to the average reading and math scores at THS, there was a significant decrease in percentages passing math and reading as well as percentage of overall passing once the THS 9th grade scores were changed to NaN and the 9th graders from THS were also left in the denominator of the percentage calculations.  When the 9th graders from THS were removed from the denominator for the percentages calculations the overall percentages for passing were within a few tenths percentage points of the original module summary.


Original School Summary:

![original_school_summary](https://user-images.githubusercontent.com/80165223/115123543-27ab4500-9f83-11eb-9b18-4eb71bbdd8dc.png)

Revised School Summary (with THS 9th graders in denominator): 

![revised_school_summary](https://user-images.githubusercontent.com/80165223/115123560-41e52300-9f83-11eb-8823-117c3275240d.png)


3.	How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to other schools?

-	When replacing the ninth graders’ scores from THS with NaN and removing them from the denominator of the percentage calculation, their position in the top 5 schools results in no change.

Original Top 5 list:

![original_top_5](https://user-images.githubusercontent.com/80165223/115123567-4d384e80-9f83-11eb-8a03-cf430ce0de02.png)


Revised Top 5 list:

![revised_top_5](https://user-images.githubusercontent.com/80165223/115123571-51fd0280-9f83-11eb-9f5c-f2d28105e8b8.png)


4.	How does replacing ninth-grade scores affect the following:


a.	Math and reading scores by grade

-	There is no impact to other schools’ scores.  THS displays NaN as displayed below for reading scores (one example):

![reading_scores_by_grade](https://user-images.githubusercontent.com/80165223/115123588-68a35980-9f83-11eb-893a-ac58698d85d7.png)


b.	Scores by school spending

-	The impact of replacing ninth grade THS scores is minimal.  The only spending category that is impacted is the spending bin $630 – 644.  Once 9th grade scores are removed (while also removing those students from the denominator) the average scores and percentage passing changed by a few tenths or hundredths points.

Original scores by spending ranges:

![orginal_spending_scores](https://user-images.githubusercontent.com/80165223/115123608-7e188380-9f83-11eb-89da-f5c7a9252c33.png)


Revised scores by spending ranges:


![revised_spending_scores](https://user-images.githubusercontent.com/80165223/115123613-81137400-9f83-11eb-9c2a-16eda10399ff.png)


c.	Scores by school size

-	The impact of replacing ninth grade THS scores is minimal.  The only school size category that is impacted is the medium size school range.  Once 9th grade scores are removed (while also removing those students from the denominator) the average scores and percentage passing changed by a few tenths or hundredths points.

Original scores by school size:


![original_school_size](https://user-images.githubusercontent.com/80165223/115123621-88d31880-9f83-11eb-9c67-db2308493138.png)


Revised scores by school size:


![revised_school_size](https://user-images.githubusercontent.com/80165223/115123628-925c8080-9f83-11eb-9217-e554781cc1ee.png)



d.	Scores by school type

-	The impact of replacing ninth grade THS scores is minimal.  The only school type category that is impacted is the Charter category.  Once 9th grade scores are removed (while also removing those students from the denominator) the average scores and percentage passing changed by a few tenths or hundredths points.

Original scores by school type:


![original_scores_school_type](https://user-images.githubusercontent.com/80165223/115123635-9b4d5200-9f83-11eb-8a49-b5a1e0d31dca.png)



Revised scores by school type:


![revised_scores_school_type](https://user-images.githubusercontent.com/80165223/115123651-a7d1aa80-9f83-11eb-8f22-a707a2cf4b74.png)




## Summary

Overall, replacing reading and math scores for 9th grade students at THS had minimal impact on the various summary reports.  This was the case for the following:

1.	District Summary
2.	School Summary
3.	Scores by school spending
4.	Scores by school size
5.	Scores by school type

The number of 9th grade students at THS with scores replaced by NaN is a small percentage of the overall dataset; therefore, the impacts were minor.  When isolating stats just for THS and the 9th graders are left in the denominator for percentage calculations, more sizable changes are observed.
