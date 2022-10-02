## File ingestion and schema validation

For this assignment the dataset selected is Kaggle Metadata uploaded on Kaggle platform. 
The datasource covers Kaggle users, competitions, datasets, kernels and more. 

The data for each topic is present in separate CSV files. To achieve the File ingestion task we needed a dataset of size greater than 2GB. 

The User Achievements data size is greater than 2 GB. The file size is 2.94 GB. 

Different methods of reading data has been implemented in this assignment. The selected methods are Dask, Pandas and Ray. 

Dask dataframe is large parallel DataFrame composed of smaller Pandas DataFrames.

Dask read the huge dataset in the least amount of time, and it was fastest. It took 0.02 seconds to read the dataset.

Ray took the maximum time of 53 seconds. Pandas read the dataset in 36.3 seconds

Later testutilty file is written to read config from YAML file and the results are validated in jupyter notebook.


Future work - 
Implement Spark to read the file and create data ingestion pipeline