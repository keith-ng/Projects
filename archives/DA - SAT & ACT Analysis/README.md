# Standardized Test Analysis

### Problem Statement
The ACT and SAT are both widely-recognised in the admission process. 
Both tests are deemed to be adequate representations of 'intelligence'. \
However, does each test per se accurately portray the level of 'intelligence' of candidates?


### Data Dictionary 
|Feature|Type|Dataset|Description|
|---|---|---|---|
|state|object|ACT/SAT|The State where recorded scores are from| 
|total_act2017|float|ACT|Average total ACT score from the year 2017|
|total_act2018|float|ACT|Average total ACT score from the year 2018|
|total_act2019|float|ACT|Average total ACT score from the year 2019|
|total_sat2017|float|SAT|Average total SAT score from the year 2017|
|total_sat2018|float|SAT|Average total SAT score from the year 2018|
|total_sat2019|float|SAT|Average total SAT score from the year 2019|
|act_diff1718|float|ACT|Difference of ACT score for years 2017 and 2018|
|act_diff1819|float|ACT|Difference of ACT score for years 2018 and 2019|
|sat_diff1718|float|SAT|Difference of SAT score for years 2017 and 2018|
|sat_diff1819|float|SAT|Difference of SAT score for years 2018 and 2019|
|act_sign1718|int|ACT|Sign of ACT score difference for years 2017 and 2018. 1 for positive & -1 for negative|
|act_sign1819|int|ACT|Sign of ACT score difference for years 2018 and 2019. 1 for positive & -1 for negative|
|sat_sign1718|int|SAT|Sign of SAT score difference for years 2017 and 2018. 1 for positive & -1 for negative|
|sat_sign1819|int|SAT|Sign of SAT score difference for years 2018 and 2019. 1 for positive & -1 for negative|


### Summary
We study on a States level whether an increase/decrease in ACT/SAT score is accompanied with the same movement in the other test. \
A conservative stance was taken where data points which recorded no changes in score for either test were omitted.

|Years|Both increase or decrease|One increase other decrease|Omitted|
|---|---|---|---|
|2017/18|15|18|9|
|2018/19|22|14|6|

Proportion of data that recorded an increase in score for one test but a decrease in the other: \
Years 2017/18: 42.86% \
Years 2018/19: 33.33% 


### Conclusion
The ACT and SAT individually may not accurately represent a candidate’s abilities.
Candidates can take both tests and apply with the better test score only.


### Recommendations
Academic Institutions can require both tests scores collectively to gain a more accurate representation of a candidate’s capabilities.
Alternatively, institutions could consider other matrices/methods to assess candidates.

