# Home-sales
home-sales
### The home-sales project makes use of SparkSQL in order to determine key metrics in the csv_file that was downloaded with the "spark.sparkContext.addFile(url)" function to have all the content avalaible to all nodes in the Spark cluster
### Specifically pyspark was used in order to work with the large data set and perform the data anlysis.

### Pyspark:
#### Temporary views "createOrReplaceTempView("")" was implemented in order to facilitate the following queries in the data analysis and allowing SQL-like syntax.
#### On "avg_by_view_rating_parquet_price" the data was previously partitioned by the "date_built" column so as to create a separate dictionary for each unique date_built value and facilitate the query. 
#### When perfoming the final query multiple times the data was cached and verified to be cached in order to store the temperary view for faster access and improve the multiple operations done later on

### Google Colab:
#### The enviorment used for the programming and running of the python home_sales code was google colab.
