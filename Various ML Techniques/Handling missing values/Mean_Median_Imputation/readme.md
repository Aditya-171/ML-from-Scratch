## Mean Median Imputation
---

Missing values are common in dealing with real-world problems when the data is aggregated over long time stretches from disparate sources,
and reliable machine learning modeling demands for careful handling of missing data. One strategy is imputing the missing values.

One of the techniques is mean imputation in which the missing values are replaced with the mean value of the entire feature column.
When the data is skewed, it is good to consider using the median value for replacing the missing values. 
The mean and median can only be calculated on numerical variables, therefore, these methods are suitable for continuous and discrete numerical variables only.

---
