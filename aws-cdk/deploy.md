# How to deploy project with `CDK` to AWS

```bash
$ cdk deploy
```
```bash
✨  Synthesis time: 8.62s

CdkAppStack: start: Building CdkAppStack Template
CdkAppStack: success: Built CdkAppStack Template
CdkAppStack: start: Publishing CdkAppStack Template (current_account-current_region)
CdkAppStack: success: Published CdkAppStack Template (current_account-current_region)
CdkAppStack: deploying... [1/1]
CdkAppStack: creating CloudFormation changeset...
CdkAppStack | 0/2 | 16:39:32 | REVIEW_IN_PROGRESS   | AWS::CloudFormation::Stack | CdkAppStack User Initiated
CdkAppStack | 0/2 | 16:39:38 | CREATE_IN_PROGRESS   | AWS::CloudFormation::Stack | CdkAppStack User Initiated
CdkAppStack | 0/2 | 16:39:40 | CREATE_IN_PROGRESS   | AWS::CDK::Metadata         | CDKMetadata/Default (CDKMetadata) 
CdkAppStack | 0/2 | 16:39:41 | CREATE_IN_PROGRESS   | AWS::CDK::Metadata         | CDKMetadata/Default (CDKMetadata) Resource creation Initiated
CdkAppStack | 1/2 | 16:39:41 | CREATE_COMPLETE      | AWS::CDK::Metadata         | CDKMetadata/Default (CDKMetadata) 
CdkAppStack | 2/2 | 16:39:42 | CREATE_COMPLETE      | AWS::CloudFormation::Stack | CdkAppStack 

 ✅  CdkAppStack

✨  Deployment time: 12.65s

Stack ARN:
arn:aws:cloudformation:ap-southeast-1:195608******:stack/CdkAppStack/dc3e1e70-2026-11f0-a0ab-06c7d5e93c9f

✨  Total time: 21.26s
```

## Succes case
```bash
Bundling asset HonoStack/lambda/Code/Stage...

  cdk.out\bundling-temp-42a89722db7abe0b61d08977ff05f02d1622f9d3c2e6a415e550ca12a04d9f27-building\index.js  55.6kb

⚡ Done in 17ms

✨  Synthesis time: 10.1s

HonoStack: start: Building lambda/Code
HonoStack: success: Built lambda/Code
HonoStack: start: Building HonoStack Template
HonoStack: success: Built HonoStack Template
HonoStack: start: Publishing lambda/Code (1956086xxxxxx-ap-southeast-1)
HonoStack: start: Publishing HonoStack Template (1956086xxxxxx-ap-southeast-1)
HonoStack: success: Published HonoStack Template (1956086xxxxxx-ap-southeast-1)
HonoStack: success: Published lambda/Code (1956086xxxxxx-ap-southeast-1)
HonoStack: deploying... [1/1]
HonoStack: creating CloudFormation changeset...
HonoStack | 0/9 | 00:09:49 | UPDATE_IN_PROGRESS   | AWS::CloudFormation::Stack  | HonoStack User Initiated
HonoStack | 0/9 | 00:09:53 | UPDATE_IN_PROGRESS   | AWS::Lambda::Function       | lambda (lambda8B5974B5) 
HonoStack | 1/9 | 00:10:00 | UPDATE_COMPLETE      | AWS::Lambda::Function       | lambda (lambda8B5974B5) 
HonoStack | 2/9 | 00:10:03 | UPDATE_COMPLETE_CLEA | AWS::CloudFormation::Stack  | HonoStack 
HonoStack | 3/9 | 00:10:03 | UPDATE_COMPLETE      | AWS::CloudFormation::Stack  | HonoStack 

 ✅  HonoStack

✨  Deployment time: 23.66s

Outputs:
HonoStack.ApiEndpoint = https://xxxx.execute-api.ap-southeast-1.amazonaws.com/prod/
HonoStack.tryhonoapiEndpoint6DC78BD3 = https://xxxx.execute-api.ap-southeast-1.amazonaws.com/prod/
Stack ARN:
arn:aws:cloudformation:ap-southeast-1:1956086xxxxxx:stack/HonoStack/1e5c3c90-22bd-11f0-a0cd-02e6a5352f67

✨  Total time: 33.75s
```

## Deploy with options
```bash
$ cdk deploy --require-approval never
```
