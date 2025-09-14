# Securing Data in AWS S3 Buckets

## Introduction

In this project, you'll learn how to secure data in AWS S3 buckets. S3 is a scalable storage service, and securing your data is crucial. We'll cover creating S3 buckets, setting bucket policies, enabling encryption, and implementing best practices for securing your S3 data.

## Pre-requisites

- Basic understanding of cloud computing
- An AWS account (free tier available)
- Basic knowledge of command-line interface (CLI)

## Lab Set-up and Tools

1. **AWS Account**: Sign up for a free AWS account if you dont have one.
2. **AWS Management Console**: Access to the AWS Management Console.
3. **AWS CLI**: Install the AWS Command Line Interface (CLI) on your local machine.

## Exercises

### Exercise 1: Create an S3 Bucket

#### Steps

1. Log in to the [AWS Management Console](https://aws.amazon.com/console/).
2. Navigate to the S3 Dashboard.
3. Click on "Create bucket".
4. Configure the bucket settings:
    - Bucket name: `my-secure-bucket`
    - Region: Select a region
    - Block all public access: Enable
5. Click "Create bucket".

#### Expected Output

- An S3 bucket `my-secure-bucket` created with public access blocked.

### Exercise 2: Enable Bucket Versioning

#### Steps

1. Navigate to the S3 Dashboard.
2. Select the bucket `my-secure-bucket`.
3. Click on "Properties".
4. Scroll down to "Bucket Versioning" and click "Edit".
5. Enable versioning and save changes.

#### Expected Output

- Versioning enabled for the S3 bucket `my-secure-bucket`.