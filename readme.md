# CloudForecast - CloudFormation Demonstration
This repo contains a sample CloudFormation configuration that sets up an EC2 instance behind an ELB. It is designed to demonstrate using tags to help system administrators keep their resources organized and maintained.

## Enforcing tags
- Install [cfn-lint](https://github.com/aws-cloudformation/cfn-python-lint)
- Run cfn-lint with the `TagsRequired.py` rule: `cfn-lint template.json -a ./`

## Deploying this
- Install and set up the AWS CLI
- Create the stack: `aws cloudformation create-stack --template-body ./template.json --stack-name=cf-test`
