# How to configure node version and re-deploy

## Update `serverless.yml` configure with node from `nodejs18.x` to `nodejs22.x`
```bash
org: prawee
app: greet
service: greet
frameworkVersion: '3'

provider:
  name: aws
  runtime: nodejs22.x

functions:
  api:
    handler: index.handler
    events:
      - httpApi:
          path: /
          method: get
``

## Re deploy
```bash
PS D:\code\try-serverless\greet> serverless deploy

Warning: Invalid configuration encountered
  at 'provider.runtime': must be equal to one of the allowed values [dotnet6, go1.x, java21, java17, java11, java8, java8.al2, nodejs14.x, nodejs16.x, nodejs18.x, nodejs20.x, provided, provided.al2, provided.al2023, python3.7, python3.8, python3.9, python3.10, python3.11, ruby2.7, ruby3.2]

Learn more about configuration validation here: http://slss.io/configuration-validation

Deploying greet to stage dev (us-east-1)
✔ Your AWS account is now integrated into Serverless Framework Observability
✔ Serverless Framework Observability is enabled

✔ Service deployed to stack greet-dev (65s)

dashboard: https://app.serverless.com/prawee/apps/greet/greet/dev/us-east-1
endpoint: GET - https://umfo2xkq24.execute-api.us-east-1.amazonaws.com/
functions:
  api: greet-dev-api (204 kB)

1 deprecation found: run 'serverless doctor' for more details
PS D:\code\try-serverless\greet>
```
