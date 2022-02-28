## Section 2

## • What is a Data Lake? Explain its benefits, how it differs from a data warehouse, and how it might benefit a client. 

Data Lake general focus is to store high volume and high variety of structured and unstructured data. Data lake ability to house large amount of unstructured and structured data allows for the usage of information to be utilized for the purpose of machine learning, user profiling and data discovery. As compared to Data Warehouse main focus on structured data which is useful for reporting, data visualization, dashboards and business intelligence. Data Lake allows for more exploration and research from Data scientists in order to find insights, undiscovered correlational, and ad hoc investigation of information from structured and unstructured data. 
	
## • Explain serverless architecture.  What are its pros and cons?
	• Pros
		○ Scalability
		○ Focus on application not infrastructure 
		○ Pricing 
			§ Reduced overhead
		○ Easier to set up environments
		
	• Cons
		○ Private APIs
		○ Dependent on 3rd parties
		○ Time out have a cut off of 300s timeout limits
		○ Don't have overall control
		
## • Please provide a diagram of the ETL pipeline from Section 1 using serverless AWS services. Describe each component and its function within the pipeline.

	1. CSV file (DATA.csv) --> AWS Crawler --> S3 source bucket --> Amazon Glue --> Amazon Athena
	2. S3 target bucket S3 Bucket is created and CSV is uploaded into the source bucket
		a. Establish the AWS Crawler
			i. Automatically create a table based on CSV
			ii. Automatically detect number of columns and their data types from the DATA.csv
		b. Amazon Glue does ETL to S3 target bucket
			i. Target mapping from source and do any necessary transformation
			ii. Run the job to move to S3 target bucket
		c. Amazon Athena in order to query the newly ETL data
			
			
## • Describe modern MLOps and how organizations should be approaching management from a tool and system perspective.
MLOps would focus on establishing data lakes through providing data as structured and unstructured in order to make it more efficiently for data scientists to access the data in the programming language of there choosing. Since MLOps can extract and load the raw data into a data lake, which can give free will to a data scientist to transform the data into what ever format they feel is useful for exploratory investigation and analysis. MLOps jobs is to speed up the data pipeline for data scientists.

