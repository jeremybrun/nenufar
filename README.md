# nenufar
A datalake based full storage and integration solution for timeseries data
Maintainer: Jeremy Brun jeremy.brun(at)gmail.com

# Proof on concept (v0.1) aims
* FireHose to ingest timeseries data
* S3 to store the timeseries as JSON line file gz (compaticle with Athena and S3 Select)

## MVP (v0.2) aims (each feature adding +0.01 to version #)
* CloudFormation (or maybe another system) to automatically spin/update a system
* AWS Lambda to analyse input data, update the metadata repo and push data to S3
* AWS glue ETL to manage datalake cascading
* AWS RDS to store and search metadata
* AWS Gateways / AWS Lambda / S3 Select to interogate the metadata DB & dalalake

# Full Release (v1.0) aims 
* NodeRED to transform, enrich and route incoming data
* A webpage accessing the AWS Gateway API and do metadata searches / data inquiries
* OAuth2 compatible authentication / autorisation to be designed


