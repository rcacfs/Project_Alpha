# Week 7 - Route53, cloudfront, WAF

## Overview

This project involves setting up a scalable and secure infrastructure on AWS. The tasks are divided into building blocks, each dependent on the previous one:

## Task 1: DNS Setup with Amazon Route 53

- **Objective:** Establish a scalable Domain Name System (DNS) using Amazon Route 53.
- **Documentation:**

Amazon Route 53 is a scalable and highly available Domain Name System (DNS) web service designed to route end-user requests to globally distributed endpoints.

### You'll need the following for this task:

1. An AWS Account with the necessary permissions.
2. Either
- Option 1: Terraform installed on the local machine
- Option 2: AWS Management Console access
- Option 3: AWS Command Line Interface (CLI) installed on the local machine

### Steps

#### Option 1: Terraform

1. Route 53 Configuration:
- Establish a connection to your AWS account in the Terraform script or CLI.
- Define a Route 53 hosted zone for your domain.

2. DNS Records:
- Specify DNS records, such as A records, to map domain names to corresponding IP addresses or endpoint URLs.
- Associate these records with the Route 53 hosted zone.

#### Option 2: AWS Management Console

1. Create Hosted Zone:
- Open the AWS Management Console and navigate to Route 53.
- Create a new hosted zone for your domain.

2. Add DNS Records:
- Within the hosted zone, add DNS records to map domain names to specific resources.
- Configure TTL (Time to Live) and other settings as needed.

#### Option 3: AWS Command Line Interface (CLI)

1. Create Hosted Zone:

```bash
aws route53 create-hosted-zone --name your_domain.com --caller-reference "$(date)"
```

2. Add DNS Records:
```bash
aws route53 change-resource-record-sets --hosted-zone-id your_hosted_zone_id --change-batch file://change_batch.json
```
Create a JSON file (change_batch.json) specifying the DNS record changes.

  [Route 53 Documentation](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/Welcome.html)


