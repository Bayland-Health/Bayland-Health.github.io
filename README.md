# Welcome to the Bayland Health Data Documentation

 
## Tech Stack Overview

Languages and Libraries:

 - [Python](https://www.python.org/) - Our primary programming language
 - [Streamlit](https://www.streamlit.io) - Primary framework for web app development
 - [Pandas](https://pandas.pydata.org/) - Data wrangling library
 - [Vega-Altair](https://altair-viz.github.io/) - Interactive data visualization library 
 - [Boto3](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html) - Boto3 AWS Python CDK for interaction with AWS services

Infrastructures:

 - [Amazon RDS Aurora](https://aws.amazon.com/rds/aurora/) - Our primary data relational data store **MySQL Serverless**
 - [AWS Lambda](https://aws.amazon.com/lambda/) - Serverless compute resources
 - [Amazon ECS](https://aws.amazon.com/ecs/) - Container deployment platform
 - [Amazon S3](https://aws.amazon.com/s3/) - Data Lake and large object store
 - [Amazon Athena](https://aws.amazon.com/athena/) -  To initiate Athena SQL and PySpark jobs against S3 buckets
 - [Amazon SQS](https://aws.amazon.com/sqs/) - Queuing for transactional ingestion and in-transit integrity control
 - [Amazon SNS](https://aws.amazon.com/sns/) - Data pub/sub service for alerts, notifications, and data fan-out
 - [AWS Step Functions](https://aws.amazon.com/step-functions/) - For serverless orchestration and distributed application build
 - [Amazon API Gateway](https://aws.amazon.com/api-gateway/) - For building APIs and streamlining data connections
 - [Amazon Redshift](https://aws.amazon.com/redshift/) - For data warehousing and more powerful analytical processing
 - [AWS Glue](https://aws.amazon.com/glue/) - For data ingestion, ETL pipelines, and crawlers
 - [Amazon Cognito](https://aws.amazon.com/cognito/) - Access control and active directory
 - [AWS ELB](https://aws.amazon.com/elasticloadbalancing/) - Application Load Balancer for traffic load balancing
 - [AWS WAF](https://aws.amazon.com/waf/) -  For extra security measurements against malicious attacks



## Bayland Health Organization Cloud (BHOC)
By utilizing public cloud services such as AWS, we can deploy and scale our data infrastructure in a short amount of time.


## DPL Management System (DMS)
DPL Management System utilizes the existing cloud infrastructure and data to democratize data share and data analytics for the entire company. Many of my colleagues suffered from slow and complicated reporting methods in the past. A simple query about the total number of units sold yesterday will require logging into three different accounts finding the corresponding numbers and adding them together, which could take anywhere between 10 to 30 minutes depending on the complexity. Right now with DMS, we can present ready-to-use data from our database with caching enabled to shorten this querying process to less than a half second. 
## Bayland Health Models Repository (BHMR)

We are actively working on building a regression model based on the Search Rank dataset, stored in S3, and the Search Query dataset stored in RDS aurora. The model will take ranking as a parameter and produce search volume as output. Based on this model, we can utilize the Amazon Search Term Report with daily granularity on search rank to predict the search volume. 
We will continue to refine this model and uses different special dates to make seasonal adjustment accordingly.
