# Packer AMI build
This script creates an AMI on a local Agent.  

## Requirements
* An AWS account with permissions to create EC2 instances and AMIs
* [Packer](https://www.packer.io/)

## Usage Instructions

1. Ensure your aws credentials have been configured.  These scripts expect to use [Automatic Lookup](https://www.packer.io/docs/builders/amazon.html#specifying-amazon-credentials).  To use a profile other than default, set the env variable `AWS_PROFILE` to the profile name.
1. Clone or download this repo
1. In the repo folder run 
    ```
    packer build deploy-image.json
    ```
1. Go make a cup of coffee
1. Once finished, check the output for successful test results.
1. Your AMI is now ready to launch
