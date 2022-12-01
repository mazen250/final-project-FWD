# WEBSITE LINK

- [AWS](http://mazen-udagram.s3-website-us-east-1.amazonaws.com)

# AWS SERVICES AND RESOURCES

## RDS (Relational Database Service)

- create rds instance
- make it publicly accessible
- change the vpc security group to allow access from anywhere
- change inbound rules to allow access from anywhere
- save the endpoiny and port
- image found in the aws-images folder

## S3 (Simple Storage Service)

- create s3 bucket named "mazen-udagram"
- make it public
- in the properties tab, enable static website hosting
- in the permissions tab, add a bucket policy to allow public access
- used aws cli to copy the build folder to the bucket

## IAM (Identity and Access Management)

- create a user named "mazen"
- give it programmatic access
- give it administrator access
- save the access key and secret key

## Elastic Beanstalk

- create a new application named "udagram-api"
- create a new environment named "udagram-api-env"
- use eb cli to initialize the environment
- use eb cli to deploy the application
- use eb cli to open the application in the browser
- configure the environment variables in the environment configuration
