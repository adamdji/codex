<!-- omit in toc -->
# AWS

<!-- omit in toc -->
## Index

- [General](#general)
- [Analytics](#analytics)
  - [Elasticsearch](#elasticsearch)
- [Security](#security)
- [Compute](#compute)
  - [EC2](#ec2)
  - [Lightsail](#lightsail)
  - [Lambda](#lambda)
  - [ECS](#ecs)
  - [Elastic Beanstalk](#elastic-beanstalk)
- [Databases](#databases)
  - [DynamoDB](#dynamodb)
  - [RDS](#rds)
  - [Redshift](#redshift)
  - [Aurora](#aurora)
  - [ElastiCache](#elasticache)
- [Developer Tools](#developer-tools)
  - [CodeCommit](#codecommit)
  - [CodePipeline](#codepipeline)
  - [CodeBuild](#codebuild)
  - [CodeDeploy](#codedeploy)
- [Management](#management)
  - [CloudFormation](#cloudformation)
  - [CloudWatch](#cloudwatch)
  - [Systems Manager](#systems-manager)
  - [CloudTrail](#cloudtrail)
- [Networking and Content Delivery Services](#networking-and-content-delivery-services)
  - [Virtual Private Cloud (VPS)](#virtual-private-cloud-vps)
  - [Direct Connect](#direct-connect)
  - [Route 53](#route-53)
  - [Elastic Load Balancing](#elastic-load-balancing)
  - [CloudFront](#cloudfront)
- [Storage Services](#storage-services)
  - [Elastic Block Storage (EBS)](#elastic-block-storage-ebs)
  - [Elastic File System (EFS)](#elastic-file-system-efs)
  - [S3](#s3)
  - [Glacier](#glacier)

## General

- Only use Root for billing, and deletion
- Set alarms to send SNS messages if a billing alarm goes up
- Secure root and IAM with different types of MFA (i.e. physical code, phyiscal key, virtual code)

## Analytics

### Elasticsearch

## Security

## Compute

### EC2

- [EC2Instances.info](EC2Instances.info) has pricing information.
- Different types of instances and categories for different workloads (T3, A1)
- Reserved Instances: Coupon to reduce instance cost by paying upfront, very flexible in timings, but no refunds.
- Custom security policies for inbound & outbound rules
- AMI Snapshots to scale up or backup server

### Lightsail

### Lambda

### ECS

### Elastic Beanstalk

## Databases

### DynamoDB

### RDS

### Redshift

### Aurora

### ElastiCache

## Developer Tools

### CodeCommit

### CodePipeline

### CodeBuild

### CodeDeploy

## Management

### CloudFormation

### CloudWatch

### Systems Manager

### CloudTrail

## Networking and Content Delivery Services

### Virtual Private Cloud (VPS)

### Direct Connect

### Route 53

### Elastic Load Balancing

### CloudFront

## Storage Services

### Elastic Block Storage (EBS)

> Primary storage service for EC2

### Elastic File System (EFS)

> Similar to a NAS; mount a share drive across EC2 instances

### S3

> Directly share assests to users across URLs

### Glacier
