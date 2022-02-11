# CloudFix AWS Permissions Checker

This tool usesthe AWS IAM Simulator API to check if you have appropriate permissions to run the CloudFix Configuration for your account. 

## Running the tool

#### Step 1

Click the [DevSpaces] button to launch the runtime environment for the tool

#### Step 2
Configure the AWS CLI tool with your credentials

```
aws configure
```

#### Step 3

Edit the config.yml file and replace {account_id} with your AWS user_id. 

#### Step 4

Run the checker

```
aws-iam-tester --write-to-file
```

If any permissions are missing, the details will be found in the ./results folder.

<br>

### Credits
<br>

[AWS IAM Tester tool](https://github.com/gercograndia/aws-iam-tester)
