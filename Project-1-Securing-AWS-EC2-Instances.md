# Introduction to Cloud Security: Securing AWS EC2 Instances

## Introduction

In this project, you'll learn how to secure AWS EC2 instances. We'll cover basic concepts like setting up security groups, configuring key pairs for SSH access, and implementing best practices for securing EC2 instances.

## Pre-requisites

- Basic understanding of cloud computing
- An AWS account (free tier available)
- Basic knowledge of command-line interface (CLI)

## Lab Set-up and Tools

1. **AWS Account**: Sign up for a free AWS account if you don't have one.
2. **AWS Management Console**: Access to the AWS Management Console.
3. **AWS CLI**: Install the AWS Command Line Interface (CLI) on your local machine.
4. **SSH Client**: Install an SSH client (e.g., OpenSSH, PuTTY) on your local machine.

## Exercises

### Exercise 1: Launch an EC2 Instance

#### Steps

1. Log in to the [AWS Management Console](https://aws.amazon.com/console/).
2. Navigate to the EC2 Dashboard.
3. Click on "Launch Instance".
4. Choose an Amazon Machine Image (AMI) (e.g., Amazon Linux 2 AMI).
5. Select an instance type (e.g., t2.micro which is free tier eligible).
6. Configure instance details (leave default settings).
7. Add storage (leave default settings).
8. Add tags (optional).
9. Configure Security Group:
    - Create a new security group.
    - Add a rule to allow SSH (port 22) from your IP.
10. Review and launch the instance.
11. Select "Create a new key pair", name it, and download the key pair.
12. Launch the instance.

#### Expected Output

- An EC2 instance running and accessible via SSH.

### Exercise 2: Connect to Your EC2 Instance

#### Steps

1. Open your terminal or SSH client.
2. Navigate to the directory where your key pair is stored.
3. Change the permissions of your key pair file:
    ```bash
    chmod 400 your-key-pair.pem
    ```
4. Connect to your instance using the public DNS:
    ```bash
    ssh -i "your-key-pair.pem" ec2-user@your-instance-public-dns
    ```

#### Expected Output

- Successful SSH connection to your EC2 instance.