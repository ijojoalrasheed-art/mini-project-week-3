First, the dataset contains user information such as age, income, city, and signup time. It had several issues like missing or unusual values, inconsistent city names, 
and very large values in age and income. So I cleaned the data by replacing the unusual values with NaN,
converting the numerical and date columns to the correct types, adding a log transformation for income to reduce the impact of large values,
and filling the missing values with the median while creating indicator columns to show where data was originally missing.
After that, I capped the outliers and standardized the city names into  a consistent format, and adjusted the dates to the same time zone.
I chose these steps because they preserve most of the data and reduce the effect of errors,
but there are trade-offs such as losing some detail from extreme values and slightly reducing variability when imputing missing data, and some rare cases may still not be fully covered by the city mapping.
