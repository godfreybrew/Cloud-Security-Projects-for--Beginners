# Google Cloud Platform Basics: Configuring IAM Policies

## Introduction

In this project, you'll learn how to configure Identity and Access Management (IAM) policies on Google Cloud Platform (GCP). IAM policies are crucial for managing access to your GCP resources. We'll cover setting up a GCP project, creating service accounts, assigning roles, and implementing best practices for IAM.

## Pre-requisites

- Basic understanding of cloud computing
- A Google Cloud Platform (GCP) account (free tier available)
- Basic knowledge of command-line interface (CLI)

## Lab Set-up and Tools

1. **GCP Account**: Sign up for a free GCP account if you don't have one.
2. **Google Cloud Console**: Access to the Google Cloud Console.
3. **Google Cloud SDK**: Install the Google Cloud SDK on your local machine.

## Exercises

### Exercise 1: Set Up a GCP Project

#### Steps

1. Log in to the [Google Cloud Console](https://console.cloud.google.com/).
2. Click on the project drop-down and select "New Project".
3. Name your project `my-gcp-project` and click "Create".

#### Expected Output

- A new GCP project `my-gcp-project` created.

### Exercise 2: Enable Billing and APIs

#### Steps

1. Navigate to the "Billing" section in the Google Cloud Console.
2. Link your project to a billing account.
3. Navigate to the "APIs & Services" section.
4. Enable necessary APIs (e.g., Compute Engine API).

#### Expected Output

- Billing enabled and essential APIs activated for the project.

### Exercise 3: Create a Service Account

#### Steps

1. Navigate to "IAM & Admin" and select "Service accounts".
2. Click on "Create Service Account".
3. Configure the service account:
    - Name: `my-service-account`
    - ID: `my-service-account`
4. Assign roles to the service account (e.g., Viewer role).
5. Click "Done".

#### Expected Output

- A service account `my-service-account` created with the Viewer role.

