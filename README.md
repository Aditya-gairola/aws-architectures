# aws-architectures




## AWS Airprt DATA Mangement Steps

### Step 1
Build an operational data management system with systems of record such as schedules,near real-time flight information, traveler check-ins,
transactions in the airport

### Step 2
Collect addresses, demographics, and other public data sets with AWS DATA EXCHANGE. Ingest private data sets with AWS STORAGE GATEWAY and 
AWS TRANFER FAMILY

### Step 3
Optionally, enhance the baggage system with a radio frequency identification(RFID) type of sortation and tracking system. Or, leverage the 
bar code scanners and baggage sortation events. Combine AWS IoT GREENGRASS, AWT IoT Core, and Amazon Kinesis to ingest sortation events.

### Step 4
provide staging for ingesting all batch and near real-time data using cost-effective storage classes in Amazon Simple Storage Service(Amazon S3).

### Step 5
Use Amazon EMR and WS Glue to transform your data. Use open standards to build the data lake using the same data as the operational data management
system. Use a read pattern schema to make the raw data and curated data readily available for all user roles.

### Step 6
Build all reportable data sets in Amazon S3, and leverage Amazon Redshift, Amazon Athena, and Amazon QuickSight for analytics.
optionally, build data marts in Amazon Redshift for heavily used anaytics. For miscellaneous requirements, publish the AWS Glue Data Catalog, and
use Athena for analysis using the data lake built in Step 5

### Step 7
Use Amazon Sagemaker to provide standard artificial intelligence and machine learning(AI/ML) models for operational analytics. You can 
also use SageMaker to build your own models on top of the data.

### Step 8 
Use purpose-built databases like Amazon DynamoDB, and serverless services like AWS Lambda amd Amazon API Gateway, to deliver microservices 
and events for operational data stores.
Build near real-time operational dashboards and customer applications using these microservices.

### Step 9
Leverage Amazon DynamoDB Streams and AWS Step Functions to publish flight and customer events to downstreams systems, like baggage reconciliation
and ground transportation.
