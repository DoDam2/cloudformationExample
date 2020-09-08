# CF Stack의 확장
## Cross-Stack
* Network cross-stack:
<https://s3.amazonaws.com/cloudformation-examples/user-guide/cross-stack/SampleNetworkCrossStack.template>
* Web app cross-stack:
<https://s3.amazonaws.com/cloudformation-examples/user-guide/cross-stack/SampleWebAppCrossStack.template>
* 현재 폴더에 있는 것은 Bug Patch 한 것.

## Nested Stack
* 중첩 스택 작업 : <https://docs.aws.amazon.com/ko_kr/AWSCloudFormation/latest/UserGuide/using-cfn-nested-stacks.html>
* Example :  https://docs.aws.amazon.com/ko_kr/AWSCloudFormation/latest/UserGuide/aws-properties-stack.html
```yaml
AWSTemplateFormatVersion: "2010-09-09"
Resources:
  myStackWithParams:
    Type: AWS::CloudFormation::Stack
    Properties:
      TemplateURL: "https://s3.amazonaws.com/cloudformation-templates-us-east-2/EC2ChooseAMI.template"
      Parameters:
        InstanceType: "t1.micro"
        KeyName: "mykey"
```

## StackSet
* [AWS CloudFormation StackSets로 작업](https://docs.aws.amazon.com/ko_kr/AWSCloudFormation/latest/UserGuide/what-is-cfnstacksets.html)
