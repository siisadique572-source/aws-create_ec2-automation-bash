# Interactive AWS EC2 Instance Automation Script

A professional, interactive Bash script that guides you step-by-step to provision an Amazon EC2 instance with strict input validation, automatic AWS CLI installation, and live state tracking.

##  Features

-   Interactive User Input:   Dynamically prompts the user for AWS details (AMI ID, Key Name, Subnet, etc.) at runtime.
-   Strict Input Validation:   Uses Regex patterns to verify if the entered AMI ID (`ami-*`), Subnet ID (`subnet-*`), and Security Group ID (`sg-*`) are valid before moving forward.
-   Automated Prerequisites:   Checks if `aws` CLI is installed. If missing, it automatically installs AWS CLI v2.
-   Fail-Safe Execution:   Uses `set -euo pipefail` to catch errors and prevent partial or broken resource creation.
-   Live State Polling:   Monitors the AWS API and waits dynamically until the instance transitions into a fully `running` state.

##  Prerequisites

Before executing the script, make sure you have:
1. An AWS Account.
2. Configured your local credentials via `aws configure`.
3. Created an SSH Key Pair in your target AWS region.

##  How to Use

1.  Clone the repository:**
   ```bash
   git clone [https://github.com/siisadique572-source/aws-create_ec2-automation-bash.git](https://github.com/siisadique572-source/aws-create_ec2-automation-bash.git)

   cd aws-create_ec2-automation-bash

