# Surfs Up Analysis

## Overview of Surfs Up Analysis:

W. Avy would like us to continue with our analysis by including more information on temperature trends before opening the surf shop.  Specficially he is looking for data from the months in June and December to confirm whether the business is sustainable to operate all year round.



## Resources
- [Hawaii_Weather_Data](https://github.com/sbretag/surfs_up/blob/main/hawaii.sqlite)
- [Analysis Code](https://github.com/sbretag/surfs_up/blob/main/SurfsUp_Challenge.ipynb)
- Software: Python 3.8.8
- Data Libraries: Pandas, Datetime, SqlAlchemy

## Results

### June Temp Statistical Results
![](https://github.com/sbretag/surfs_up/blob/main/Resources/june_results.png)

### Dec Temp Statistical Results
![](https://github.com/sbretag/surfs_up/blob/main/Resources/dec_results.png)

### Key Differences

1. Although there are a significant amount of observations for both December and June periods with 1500+, June has roughly 200 more observations than December.  Given that December has one more day than June I question the data source since weather observations should be fairly automated.  
2.The max temps for December and June are relatively close to each other which suggests that even December can produce higher temps, even if they are infrequent outliers
3. The opposite could be said about the minimums as the coldest days in December are much more colder than the coldest days in June

## Summary
- High Level Summary
  - Overall the average temps between June and December are not that much different, only by 3-4 degrees.  The same can be said about the standard deviations, 25%, 50%, and 75% percentiles.  Although the coldest days in Dec are are almost 8 degress lower than that in June, since the means are relatively close to each other it would suggest that this is relatively infrequent.  Looking at just June and December, I believe it they have evidence that the business would be sustainable.  With that said, I believe more testing can be done to further validate and confirm, see proposals below.  
- Additional Queries to run
  - Using two months to test whether the business is sustainable all year could result in incorrect information, I would suggest running a query that would look at each month to identify the extremes which may differ from June & December
  - Another recommendation would be to limit the query to the past two years rather than all years to see if more recent climate trends have different results
