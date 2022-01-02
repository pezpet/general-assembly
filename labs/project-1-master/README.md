# Executive Summary for Project 1
## Problem Statement
SAT and ACT prep for high school students varies widely given different levels of access to materials, tutors and time available for extra studying, among others. It has been stated in media that households with higher incomes have unfair advantages in standarized testing. We are going to look at county level data for California and determine how much are SAT and ACT scores in California related to median household income levels?
## Description of data
For this project we have used two of the provided data sets:
- SAT scores for California schools in 2019
    - Size: 2580 rows, 26 columns
    - Source: (https://www.cde.ca.gov/ds/sp/ai/)
    - Data Dictionary: (https://www.cde.ca.gov/ds/sp/ai/reclayoutsat19.asp)
    - We found the most relevant features for our project to be "PctBothBenchmark12" and "PctBothBenchmark11", indexed by county. The data does not include actual SAT scores, but these features seemed useful if compared to county level income data.
- ACT scores for California schools in 2019
    - Size: 2310 rows, 18 columns
    - Source: (https://www.cde.ca.gov/ds/sp/ai/)
    - Data Dictionary: (https://www.cde.ca.gov/ds/sp/ai/reclayoutact19.asp)
    - We found the most relevant features for our project to be "AVGSCR..." columns 8 through 11. With these average scores we were able to estimate composite scores by county to compare with income levels.
>To complete our analysis we have included a data set for household incomes in California (this data is segmented by race, but a total is given for each county, making it useful without icluding race features):
- Household income by race in California:
    - Size: 2494 rows, 9 columns
    - Source: (https://datausa.io/api/data?Geography=04000US06:children&measure=Household%20Income%20by%20Race,Household%20Income%20by%20Race%20Moe&drilldowns=Race)
    - We selected the column "Household Income by Race" and selected all races to produce a data set of median household incomes by counties in California, for 2019
## Primary Findings & Conclusions
Percentages of SAT takers in California with scores above benchmark, and ACT composite scores, are positively correlated to the median household income of the county where the test takers go to school.

Among ACT scores, the Math average score showed the highest correlation to Household income.

This can be seen as confirmation that households with higher incomes can expect to have children with higher SAT/ACT scores.

## Next Steps
This analysis can be furthered by including more granular data related to the selected data sets:
- Actual SAT scores
- More detailed income data per county (only the median was used in this project)