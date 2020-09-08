# Aws Cli
## Install on Ubuntu
```
sudo apt update -y
sudo apt install -y awscli
```

## Configure
1. [AWS IAM Console](https://console.aws.amazon.com/iam) 에서 유저 생성
2. "PowerUserAccess" 권한 추가
3. Tocken 생성
4. Configure
```
aws configure
```

## Examples
### AWS cli command
```
aws cloudformation help
aws cloudformation list-stacks --stack-status-filter CREATE_COMPLETE
aws cloudformation create-stack --stack-name s11 --template-body file://./minimal.yaml
aws cloudformation describe-stacks --stack-name mu-iam-common
aws cloudformation get-template --stack-name mu-iam-common
aws cloudformation validate-template --template-body file://./minimal.yaml
aws cloudformation delete-stack
```
### Bash Script
```
. create.sh
. check.sh
. delete.sh
```
