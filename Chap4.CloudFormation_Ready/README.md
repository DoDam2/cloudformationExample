# CloudFormation 준비
## IAM
* Policy Example : IAM → 정책 → 정책생성 → JSON
```
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "CreateSpecificRoleForSpecificService",
            "Effect": "Allow",
            "Action": "iam:CreateRole",
            "Resource": "arn:aws:iam::*:role/testRole",
            "Condition": {"StringLike": {"iam:AWSServiceName": "ec2.amazonaws.com"}}
        },
        {
            "Sid": "AddPoliciesToSpecificRole",
            "Effect": "Allow",
            "Action": [
                "iam:AttachRolePolicy",
                "iam:PutRolePolicy"
            ],
            "Resource": "arn:aws:iam::*:role/testRole"
        }
    ]
}
```

## CloudTrail
* AWS CloudTrail Service :  [https://ap-northeast-2.console.aws.amazon.com/cloudtrail/](https://ap-northeast-2.console.aws.amazon.com/cloudtrail/)
