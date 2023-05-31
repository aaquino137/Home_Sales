# Home_Sales

Since we are dealing with Big Data we can't use Pandas to anlyaze the data. Instead we use SparkSQL because it allows for us to deal with larger data amounts. By creating a Temporary table we are able to conduct queries oon our data. The reasoning behind using Parquets and Cache is to optimize the speed of the code being run.Originally the run time for the query was .77s. By using cached data, the speed improved to .66s. Afterwards, the data was partitioned by the "date_built" column. In comparison to the cahed data, the speed improved slightly. 
