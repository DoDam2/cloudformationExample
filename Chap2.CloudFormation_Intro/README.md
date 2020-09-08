# CloudFormation 소개
![create-stack-diagram](https://docs.aws.amazon.com/ko_kr/AWSCloudFormation/latest/UserGuide/images/create-stack-diagram.png)
## IAM
* AWS 서비스와 리소스에 대한 액세스 관리
* AWS IAM Document : [https://aws.amazon.com/ko/iam/](https://aws.amazon.com/ko/iam/)
* AWS IAM Console : [https://console.aws.amazon.com/iam/](https://console.aws.amazon.com/iam/)

## Template
### Support File
* [json](http://www.json.org)
```json
{
  "AWSTemplateFormatVersion" : "2010-09-09",
  "Description" : "A simple EC2 instance",
  "Resources" : {
    "MyEC2Instance" : {
      "Type" : "AWS::EC2::Instance",
      "Properties" : {
        "ImageId" : "ami-0ff8a91507f77f867",
        "InstanceType" : "t1.micro"
      }
    }
  }
}
```
* [yaml](http://www.yaml.org)
```yaml
AWSTemplateFormatVersion: '2010-09-09'
Description: A simple EC2 instance
Resources:
  MyEC2Instance:
    Type: AWS::EC2::Instance
    Properties:
      ImageId: ami-0ff8a91507f77f867
      InstanceType: t1.micro
```
* [Json to Yaml ](https://www.json2yaml.com) : 변환 및 검증에 활용.


## Stack
* CloudFormation의 작업 단위

## Change Set
* 스택의 리소스를 업데이트해야 하는 경우 사용
