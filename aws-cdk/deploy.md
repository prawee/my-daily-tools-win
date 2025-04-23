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
