AWS Platform
============

# AWS Global Infrastructure

Regions - Geographical area in the world where AWS resources exist, with 2 or more Availability Zones
Availability Zone - logical Data Center
Edge Locations - CDN end points for CloudFront
               - more Edge Locations than there are Regions

## Network & Content Delivery

VPC - Virtual Private Cloud
    - virtual data center
Route53 - DNS service
        - can register domains
        - 53 is the DNS port
Cloud Front - CDN network
            - edge locations caching resources
Direct Connect - connect physical data centers to AWS

## Compute

EC2 - Elastic Compute Cloud
    - VMs 
EC2 Container Service - container management service supporting Docker
Elastic Beanstalk - provision infrastructure based on type of application
Lambda - serverless code execution (functions)
Lighsail - out of the box cloud eg. create defined stack

## Storage

S3 - Object based storage
Glacier - Data archival
        - Low cost
        - No immediate retrieval
EFS - File storage which can be shared across multipe VMs
Storage Gateway - Way to connect S3 to on-premise servers

## Databases

RDS - Relational Database Service
    - MySQL, PostgresSQL, MariaDB, SQL Server, Oracle, Aurora
DynamoDB - NoSQL
Redshift - DataWarehousing Solution
Elasticacahe - Data cache

## Migration Services

Snowball - Data drive to import data from on-premise
Snowball Edge - 
DMS - Database migration service, either from on-premise or within AWS
SMS - Server Migration Services, migrate VMs to AWS

## Analytics

Athena - Run SQL queries on S3
EMR- Elastic Map Reduce Big Data processing, Hadoop based
Cloud Search
Elastic Search
Kinesis - way of streaming and analysing big data
Data Pipeline - service to move data from one location to another
Quick Sight - Business Analytics Tool with visualisations and dashboards

## Security and Identity

IAM - User, authentication and authorisation service
Inspector - installed on VMs and performs security inspection
Certificate Management - Free SSL certs for Domain names
Directory Service - connects Active Directory to AWS
WAF - Web Application Firewall 
    - application level protection
Artifacts - compliance documentation from AWS console
          - e.g. ISO certificates, etc

## Management Tools

Cloud Watch - monitors performance of AWS environment
Cloud Formation - Infrastructure as Code
Cloud Trail - audit AWS environment changes
Opsworks - Chef automation
Config - monitors environment against configuration rules and alerts
Service Catalog - catalog of authorised services by your organisation
Trusted Advisor - automated good practice recommendations based on your AWS environment/usage

## Application Services

Step Functions - Visualising what is going between applications
SWF - Simple Workflow Service
    - process management
API Gateway - create, publish and monitor APIs
AppStream - streaming Desktop applications to your users
Elastic Transcoder - changes video format to suit receiving device

## Developer Tools

CodeCommit - Git repository
CodeBuild - Build/compile code
CodeDeploy - Deploy code to EC2 instances
CodePipeline - track versions of code against environments

## Mobile Services

Mobile Hub - add, configure and design features for mobile apps
Cognito - user sign-up and login service via Social Media providers
Device Farm - test iOS apps on physical devices
Mobile Analytics - collect and analyse app usage data
Pinpoint - understand, analyse and engage with app users


## Business Productivity

WordDocs - securely store work documents in cloud
WorkMail - sending and receiving email

## IOT

iOT - IOT services

## Desktop & App Streaming

Workpaces - VDI service
AppStream 2.0 - way of streaming desktop applications to users

## AI

alexa - Voice Service in the Cloud
      - via Echo device
lex - 
Polly - text to voice service 
Machine Learing - dataset and outcome analysis
Rekognition - image analysis and recognition service

## Messaging

SNS - email or text message notifications
SQS - queue system
SES - Simple Email Service
    - send and receive emails







