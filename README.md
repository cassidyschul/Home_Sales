# Home Sales Data Analysis using SparkSQL

In this assignment, I read data from an AWS S3 bucket and stored it in a temporary table. Using SparkSQL, I analyzed the data to determine key metrics. The temporary table was cached, and the differences in run times were compared. As expected, the run times for the cached table were significantly lower than for the uncached table.

Next, the data was partitioned by the date_built column, stored in parquet format, and loaded into a temporary table. I measured and compared the query run time to that of the cached data.

When comparing parquet and cache run times, the cache run times were lower. When comparing the parquet and uncache run times, the parquet run times were lower. 
