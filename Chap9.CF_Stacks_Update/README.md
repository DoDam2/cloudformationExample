# CF Stacks Update
## LAMP 스택 생성
0. 키생성(EC2 Console에서 생성)
1. [Cloudformation Conole](https://ap-northeast-2.console.aws.amazon.com/cloudformation)접속
2. "스택 생성" 선택
3. "새 리소스 사용(표준)" 선택
4. "LAMP Stack" 선택
5. ..


## Direct 수정
* WebServer EC2 instance type을 t2.small로 수정해 봅시다.
## Change Set
1. [Cloudformation Conole](https://ap-northeast-2.console.aws.amazon.com/cloudformation)
2. "스택 작업" 선택
3. "현재 스택에 대한 변경 세트 만들기" 선택
4. "현재 템플릿 사용" 선택
5. "다음" 클릭

## Codepipeline
* [연습: 테스트 및 프로덕션 스택용 파이프라인 빌드](https://docs.aws.amazon.com/ko_kr/AWSCloudFormation/latest/UserGuide/continuous-delivery-codepipeline-basic-walkthrough.html)
