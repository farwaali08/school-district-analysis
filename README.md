# school-district-analysis

## OVERVIEW

In this analysis, the standardized test scores for 15 schools within a district were used to provide insights on performance trends and patterns. The main objective was to assist the school district with decisions regarding budget allotments and priorities.

It was later learned that the standardized test scores for ninth grade students at Thomas High School (THS) may be compromised, and after review, it was decided that the original analysis should be refactored to exclude the test scores for this group. 

In doing so, 461 students records (each, for math and reading,) were precluded from the calculations, and final analysis, which was presented to the board.

## TOOLS and RESOURCES

Raw data can be found within the "Resources" folder.

[Student Data (CSV)](https://github.com/farwaali08/school-district-analysis/blob/87c86d29c1de87fb2eb3d07676465312682ac573/Resources/students_complete.csv)

[School Data (CSV)](https://github.com/farwaali08/school-district-analysis/blob/87c86d29c1de87fb2eb3d07676465312682ac573/Resources/schools_complete.csv)

[Cleaned (CSV)](https://github.com/farwaali08/school-district-analysis/blob/87c86d29c1de87fb2eb3d07676465312682ac573/Resources/clean_students_complete.csv)

Data was analyzed using the pandas library in Python 3.9.3,, and visualized in Jupyter Notebook 6.3.0.

[Original Analysis](https://github.com/farwaali08/school-district-analysis/blob/87c86d29c1de87fb2eb3d07676465312682ac573/PyCitySchools.ipynb)

[Refactored Analysis](https://github.com/farwaali08/school-district-analysis/blob/87c86d29c1de87fb2eb3d07676465312682ac573/PyCitySchools_Challenge_starter_code.ipynb)

## RESULTS and ANALYSIS

In the first part of the refactored analysis, 461 student records (each for math and reading) were removed from the calculation, by replacing the test scores with a value of "NaN" ("not a number") as illustrated in the image below:


![alt_text](https://github.com/farwaali08/school-district-analysis/blob/57b2eb6334d7382702f0c19bd3fa3bdf1b8458e3/NaN1.png)





