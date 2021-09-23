# school-district-analysis

## OVERVIEW

In this analysis, the standardized test scores for 15 schools within a district were used to provide insights on performance trends and patterns. The main objective was to assist the school district with decisions regarding budget allotments and priorities.

It was later learned that the standardized test scores for ninth grade students at Thomas High School (THS) may be compromised, and after review, it was decided that the original analysis should be refactored to exclude the test scores for this group. 

In doing so, 461 students records (each, for math and reading,) were precluded from the calculations and the final analysis, which was presented to the board.

## TOOLS and RESOURCES

Raw data can be found within the "Resources" folder.

[Student Data (CSV)](https://github.com/farwaali08/school-district-analysis/blob/87c86d29c1de87fb2eb3d07676465312682ac573/Resources/students_complete.csv)

[School Data (CSV)](https://github.com/farwaali08/school-district-analysis/blob/87c86d29c1de87fb2eb3d07676465312682ac573/Resources/schools_complete.csv)

[Cleaned (CSV)](https://github.com/farwaali08/school-district-analysis/blob/87c86d29c1de87fb2eb3d07676465312682ac573/Resources/clean_students_complete.csv)

Data was analyzed using the pandas library in Python 3.9.3, and visualized in Jupyter Notebook 6.3.0.

[Original Analysis](https://github.com/farwaali08/school-district-analysis/blob/87c86d29c1de87fb2eb3d07676465312682ac573/PyCitySchools.ipynb)

[Refactored Analysis](https://github.com/farwaali08/school-district-analysis/blob/87c86d29c1de87fb2eb3d07676465312682ac573/PyCitySchools_Challenge_starter_code.ipynb)

## RESULTS and ANALYSIS

In the first part of the refactored analysis, 461 student records (each for math and reading) were removed from the calculation, by replacing the test scores with a value of "NaN" ("not a number") as illustrated in the image below:


![alt_text](https://github.com/farwaali08/school-district-analysis/blob/57b2eb6334d7382702f0c19bd3fa3bdf1b8458e3/NaN1.png)



A quick validation was done to ensure that all the necessary records were updated successfully:


![alt_text](https://github.com/farwaali08/school-district-analysis/blob/7737c1b38c37e0968c88b1495a9089747d2e1e45/confirmnan.png)



Once this step was completed, the script was re-executed and analyzed:


### **DISTRICT SUMMARY**

*Original Results:*

![alt_text](https://github.com/farwaali08/school-district-analysis/blob/06bf8b29ec5b0efed0cd250ed90730d528d81efc/district_summary_1.png)



*Refactored Results:*

![alt_text](https://github.com/farwaali08/school-district-analysis/blob/06bf8b29ec5b0efed0cd250ed90730d528d81efc/district_summary_2.png)


Omitting the dubious test scores did not appear to have an appreciable difference on the district summary, and further analysis will be required to determine whether the results are statistically significant. Upon initial review however, it is apparent that all performance metrics, save for the average reading score, were negatively impacted. Although the differences range from 0.1-0.2%, this can be problematic if KPI thresholds are not met.


### **SCHOOL SUMMARY**

The original school summary can be found below:

![alt_text](https://github.com/farwaali08/school-district-analysis/blob/f01c68852ace92c7335850f461e7531e874e4491/SCHOOL_SUMMARY1.png)


The revised school summary is as follows:

![alt_text](https://github.com/farwaali08/school-district-analysis/blob/f01c68852ace92c7335850f461e7531e874e4491/SCHOOL_SUM_REFAC.png)

The omitted test scores negatively impacted all performance metrics. The average test scores for both reading and math were not impacted as greatly as the passing percentages, which all dropped by nearly 30% each.


### **SCHOOL RANKINGS**

The omitted data caused THS' performance to drop, which would remove them from the Top 5 peforming schools. The Bottom 5 ranking was not impacted, however.


Original Top 5 Ranking:

![alt_text](https://github.com/farwaali08/school-district-analysis/blob/6fbf7f530e90e75ab726ccf90994125872d8b7e9/Top_5_Original.png)



### **OTHER CONSIDERATIONS**

* The "Average Math Scores by Grade & School" and "Average Reading Scores by Grade & School" categories were not impacted by this change, as the data for THS was simply replaced by a value of "NaN". Below is one example, which demonstrates that the other data has remained intact:

     > ![alt_text](https://github.com/farwaali08/school-district-analysis/blob/c636ddfc9588e2e6b0b40622b2062fa76994352e/nan_no_impact.png) 


* Additionally,
> **School Size** and **School
