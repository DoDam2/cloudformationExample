# CF Template으로 AWS Config 관리형 규칙 만들기
## Setup AWS config
* AWS Config를 사용하여 AWS 리소스의 인벤토리와 해당 리소스에 대한 구성 변경 기록의 규칙 준수 여부를 평가하는 규칙을 정의함.
* [AWS Config](https://ap-northeast-2.console.aws.amazon.com/config/) → 시작하기

## Desired-instance-type
* [AWS Config 개발자 가이드](https://docs.aws.amazon.com/ko_kr/config/latest/developerguide/WhatIsConfig.html)
* [AWS CloudFormation 템플릿으로 AWS Config 관리형 규칙 만들기](https://docs.aws.amazon.com/ko_kr/config/latest/developerguide/aws-config-managed-rules-cloudformation-templates.html)

### S3 Templates
* https://s3.amazonaws.com/aws-configservice-us-east-1/cloudformation-templates-for-managed-rules/DESIRED_INSTANCE_TYPE.template
* https://s3.amazonaws.com/aws-configservice-us-east-1/cloudformation-templates-for-managed-rules/INCOMING_SSH_DISABLED.template
* https://s3.amazonaws.com/aws-configservice-us-east-1/cloudformation-templates-for-managed-rules/restricted-ssh.template
