# aws-glue-crawler
AWS Glue crawler using Cloudformation template to scan s3 bucket.


####Getting Started with CloudFormation

Before getting going with the commands, make sure the 
```html
aws configure```
command is executed and the region is setup properly

Use the following command to list the current cloudformation templates supported in the account.
```html
aws cloudformation list-stacks
```

Use the following command to create stack from template.
```html
aws cloudformation create-stack --stack-name mystackcli1 --template-body file://./hello-cloudformation.json --debug
```

If you experience the following error when running create-stack, make sure the user
has IAM permission setup properly.
```html
InsufficientCapabilitiesException: An error occurred (InsufficientCapabilitiesException) when calling the CreateStack operation: Requires capabilities : [CAPABILITY_IAM]
```
