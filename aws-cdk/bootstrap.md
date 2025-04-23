# First step with `AWS CDK`

```bash
$ cdk bootstrap
```
```bash
 ⏳  Bootstrapping environment aws://195608******/ap-southeast-1...
Trusted accounts for deployment: (none)
Trusted accounts for lookup: (none)
Using default execution policy of 'arn:aws:iam::aws:policy/AdministratorAccess'. Pass '--cloudformation-execution-policies' to customize.
CDKToolkit: creating CloudFormation changeset...
CDKToolkit |  0/12 | 16:33:51 | REVIEW_IN_PROGRESS   | AWS::CloudFormation::Stack | CDKToolkit User Initiated
CDKToolkit |  0/12 | 16:33:56 | CREATE_IN_PROGRESS   | AWS::CloudFormation::Stack | CDKToolkit User Initiated
CDKToolkit |  0/12 | 16:33:59 | CREATE_IN_PROGRESS   | AWS::ECR::Repository       | ContainerAssetsRepository 
CDKToolkit |  0/12 | 16:33:59 | CREATE_IN_PROGRESS   | AWS::IAM::Role             | FilePublishingRole 
CDKToolkit |  0/12 | 16:33:59 | CREATE_IN_PROGRESS   | AWS::IAM::Role             | CloudFormationExecutionRole 
CDKToolkit |  0/12 | 16:33:59 | CREATE_IN_PROGRESS   | AWS::IAM::Role             | LookupRole 
CDKToolkit |  0/12 | 16:33:59 | CREATE_IN_PROGRESS   | AWS::S3::Bucket            | StagingBucket 
CDKToolkit |  0/12 | 16:33:59 | CREATE_IN_PROGRESS   | AWS::SSM::Parameter        | CdkBootstrapVersion 
CDKToolkit |  0/12 | 16:33:59 | CREATE_IN_PROGRESS   | AWS::IAM::Role             | ImagePublishingRole 
CDKToolkit |  0/12 | 16:34:00 | CREATE_IN_PROGRESS   | AWS::SSM::Parameter        | CdkBootstrapVersion Resource creation Initiated
CDKToolkit |  0/12 | 16:34:00 | CREATE_IN_PROGRESS   | AWS::IAM::Role             | FilePublishingRole Resource creation Initiated
CDKToolkit |  0/12 | 16:34:00 | CREATE_IN_PROGRESS   | AWS::ECR::Repository       | ContainerAssetsRepository Resource creation Initiated
CDKToolkit |  0/12 | 16:34:00 | CREATE_IN_PROGRESS   | AWS::IAM::Role             | CloudFormationExecutionRole Resource creation Initiated
CDKToolkit |  0/12 | 16:34:00 | CREATE_IN_PROGRESS   | AWS::IAM::Role             | ImagePublishingRole Resource creation Initiated
CDKToolkit |  0/12 | 16:34:00 | CREATE_IN_PROGRESS   | AWS::S3::Bucket            | StagingBucket Resource creation Initiated
CDKToolkit |  1/12 | 16:34:01 | CREATE_COMPLETE      | AWS::SSM::Parameter        | CdkBootstrapVersion 
CDKToolkit |  2/12 | 16:34:01 | CREATE_COMPLETE      | AWS::ECR::Repository       | ContainerAssetsRepository 
CDKToolkit |  2/12 | 16:34:01 | CREATE_IN_PROGRESS   | AWS::IAM::Role             | LookupRole Resource creation Initiated
CDKToolkit |  3/12 | 16:34:15 | CREATE_COMPLETE      | AWS::S3::Bucket            | StagingBucket 
CDKToolkit |  3/12 | 16:34:16 | CREATE_IN_PROGRESS   | AWS::S3::BucketPolicy      | StagingBucketPolicy 
CDKToolkit |  3/12 | 16:34:18 | CREATE_IN_PROGRESS   | AWS::S3::BucketPolicy      | StagingBucketPolicy Resource creation Initiated
CDKToolkit |  4/12 | 16:34:18 | CREATE_COMPLETE      | AWS::S3::BucketPolicy      | StagingBucketPolicy 
CDKToolkit |  5/12 | 16:34:18 | CREATE_COMPLETE      | AWS::IAM::Role             | FilePublishingRole 
CDKToolkit |  6/12 | 16:34:19 | CREATE_COMPLETE      | AWS::IAM::Role             | CloudFormationExecutionRole 
CDKToolkit |  6/12 | 16:34:19 | CREATE_IN_PROGRESS   | AWS::IAM::Policy           | FilePublishingRoleDefaultPolicy 
CDKToolkit |  7/12 | 16:34:19 | CREATE_COMPLETE      | AWS::IAM::Role             | ImagePublishingRole 
CDKToolkit |  7/12 | 16:34:20 | CREATE_IN_PROGRESS   | AWS::IAM::Policy           | ImagePublishingRoleDefaultPolicy 
CDKToolkit |  7/12 | 16:34:20 | CREATE_IN_PROGRESS   | AWS::IAM::Role             | DeploymentActionRole 
CDKToolkit |  8/12 | 16:34:20 | CREATE_COMPLETE      | AWS::IAM::Role             | LookupRole 
CDKToolkit |  8/12 | 16:34:21 | CREATE_IN_PROGRESS   | AWS::IAM::Policy           | FilePublishingRoleDefaultPolicy Resource creation Initiated
CDKToolkit |  8/12 | 16:34:22 | CREATE_IN_PROGRESS   | AWS::IAM::Role             | DeploymentActionRole Resource creation Initiated
CDKToolkit |  8/12 | 16:34:22 | CREATE_IN_PROGRESS   | AWS::IAM::Policy           | ImagePublishingRoleDefaultPolicy Resource creation Initiated
CDKToolkit |  9/12 | 16:34:37 | CREATE_COMPLETE      | AWS::IAM::Policy           | FilePublishingRoleDefaultPolicy 
CDKToolkit | 10/12 | 16:34:38 | CREATE_COMPLETE      | AWS::IAM::Policy           | ImagePublishingRoleDefaultPolicy 
CDKToolkit | 11/12 | 16:34:41 | CREATE_COMPLETE      | AWS::IAM::Role             | DeploymentActionRole 
CDKToolkit | 12/12 | 16:34:42 | CREATE_COMPLETE      | AWS::CloudFormation::Stack | CDKToolkit 
 ✅  Environment aws://195608******/ap-southeast-1 bootstrapped.
```
