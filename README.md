# aws-create_ec2-automation-bash
Bash script to automate AWS EC2 instance creation

# AWS EC2 Instance Automation Script

A robust Bash script to automate the installation of AWS CLI and the provisioning of an Amazon EC2 instance with strict error handling and state tracking.

##  Features

-   Automated Prerequisites:  Automatically checks for `aws` CLI and installs AWS CLI v2 if not found.
-   Strict Error Handling:  Uses `set -euo pipefail` to ensure the script exits immediately if any command fails.
-   Dynamic State Tracking:  Queries the AWS API and waits until the newly created EC2 instance is fully in a `running` state before finishing.
-   Clean Execution:   Cleans up temporary installation files automatically.

##  Prerequisites

Before running this script, ensure you have:
1. An AWS Account.
2. Configured your AWS credentials locally using `aws configure`.
3. SSH Key Pair created in your AWS region.

##  How to Use

1.   Clone the repository:

   
   - git clone https://github.com/siisadique572-source/aws-create_ec2-automation-bash.git
   
   - cd aws-create_ec2-automation-bash

