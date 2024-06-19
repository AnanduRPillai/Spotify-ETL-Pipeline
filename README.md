# Spotify-ETL-Pipeline

## Project Overview

In this project, I built an ETL (Extract, Transform, Load) Pipeline for fetching Spotify's trending playlists using the Spotify APIs.


## Extraction

-Technology: Python

-Deployment: AWS Lambda

-Storage: AWS S3

The extraction process involves writing a Python script that uses the Spotify APIs to fetch trending playlists. This script is deployed as an AWS Lambda function. The fetched raw data is stored in an S3 bucket.

## Transformation
-Technology: Python

-Deployment: AWS Lambda

-Storage: AWS S3.

For the transformation part, the data fetched from the S3 bucket by the extraction process is transformed using another AWS Lambda function. The transformed data is then stored back into an S3 bucket. AWS triggers are used to automate the extraction and transformation processes.


## Loading

-Technology: Snowflake

-Integration: AWS and Snowflake

-Analysis: PowerBI

Finally, the transformed data is loaded into Snowflake using Snowpipe. This integration between AWS and Snowflake ensures that the data flows seamlessly from S3 to Snowflake for further analysis.
