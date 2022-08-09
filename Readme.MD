## I checked the given dataset and the following are my findings:

The dataset available shows the customer reviews of hotels and resorts for the period of Aug 2018 - Aug 2019. The total number of rows is 6448 and the column consists of 3 information i.e. Review, Date, and Location. The dataset is not clean i.e. Inconsistent location- structured formatting required, inconsistent date format, Null and blank values identified.

The Review column is of qualitative nature and cannot be measured but I tried exacting common review Keywords using SQL “LIKE” function in BigQuery which helped me to extract quantitative data. 

### Keyword Used:

- Amazing
- Great
- Good
- Ok
- Average
- Terrible
- Bad
- Worst

After applying these keywords, I identified 3905 reviews that are classified as:

- Good
- Average
- Bad

### Summary

| Total Population (Row) | 6448 |
| --- | --- |
| Time Period | Aug 18- Aug 19 |
| Quantitative review data sample set acquired  | 3905 out of 6448 |

Quantitative review data sample set:

| Good | 2561 |
| --- | --- |
| Average | 1039 |
| Bad | 305 |

I observed we had 6448 end-users of our services. By aggregating the dataset I was able to measure month-on-month customer acquisition which was at a rate of 7.6% per month.

We had the highest customer acquisition in the month of Dec 2018 i.e. 9.7%. This may be because of the long Christmas holidays.

We see a fall in customer acquisition in the year 2019 by 0.9% as compared to the previous year.

I identified NULL and Blank values in the location column. They constitute 73.5% of the total population and need to be addressed swiftly.

The location column is unstructured and difficult to draw any admissible insights. After an initial level of cleaning, the following insights were found 

### In the US

Top 5 locations

1. New York
2. California
3. Florida
4. Puerto Rico
5. Michigan

Top 10 locations in the world.

1. United States of America
2. United kingdom
3. Canada
4. France
5. Italy
6. New Zealand 
7. Australia
8. Japan
9. South Africa
10. Germany

### Dashboard View

![Dashboard 1 (5).png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/7acb6951-fea1-4cd9-8103-006520e807a5/Dashboard_1_(5).png)

Link: https://public.tableau.com/views/FinalDatatestvisuals/Dashboard12?:language=en-US&:display_count=n&:origin=viz_share_link

## Conclusion

1. Monthly customer acquisition is at 7.6%.
2. December 2018, had the highest customer acquisition of 9.7%.
3. Customer reviews: Good- 65.58%, Average- 26.6%, Bad- 7.8%.
4. Top 5 locations in us- New York, California, Florida, Puerto Rico, and Michigan. Top 5 Locations in the World- USA, UK, Canada, France, and Italy.
5.  Location includes 73.5% of null and blank cells.

### Suggestions/Recommendations

1. Introduce structured formats to better capture data.
2. Introducing Geo location tracker to capture exact location automatically or using pin codes to eliminate NULL and Blanks.
3. Introduce a Quantitative scale(1-10) to better understand the customer ratings
4. Improve services at low-performing locations.
5. Introduce attractive offers during the holidays to increase customer acquisition.

---

Hope you find this insightful. 

I would also like to learn how to clean this dataset to make it much more usable such as 

- Extract keywords to separate column and categorize them accordingly.
- Cleaning the location to a universally acceptable format

By doing so, I will be able to provide more accurate customer responses and plot performance categorized areas based on location.

### Thanks!