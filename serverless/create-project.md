# How to create first project with `Serverless`

Make folder and into it first.

## Create
### Initial with `HTTP API`
```bash
PS D:\code\try-serverless> serverless

Creating a new serverless project

? What do you want to make?
  AWS - Node.js - Starter
> AWS - Node.js - HTTP API
  AWS - Node.js - Scheduled Task
  AWS - Node.js - SQS Worker
  AWS - Node.js - Express API
  AWS - Node.js - Express API with DynamoDB
  AWS - Python - Starter
  AWS - Python - HTTP API
  AWS - Python - Scheduled Task
  AWS - Python - SQS Worker
  AWS - Python - Flask API
  AWS - Python - Flask API with DynamoDB
  Other
```

### Define project name with `greet`
```bash
PS D:\code\try-serverless> serverless

Creating a new serverless project

? What do you want to make? AWS - Node.js - HTTP API
? What do you want to call this project? greet
```

### Using with serverless framework yes or not (yes) and action login on your browser to authorize
```bash
PS D:\code\try-serverless> serverless

Creating a new serverless project

? What do you want to make? AWS - Node.js - HTTP API
? What do you want to call this project? greet

✔ Project successfully created in greet folder

? Register or Login to Serverless Framework (Y/n) Y
```

### Need to deploy?
```bash
PS D:\code\try-serverless> serverless

Creating a new serverless project

? What do you want to make? AWS - Node.js - HTTP API
? What do you want to call this project? greet

✔ Project successfully created in greet folder

? Register or Login to Serverless Framework Yes
Logging into the Serverless Framework via the browser
If your browser does not open automatically, please open this URL:
https://app.serverless.com?client=cli&transactionId=kYXs6ARC0OmvgxUdFfBSq

✔ You are now logged into the Serverless Framework


✔ Your project is ready to be deployed to Serverless Dashboard (org: "prawee", app: "greet")

? Do you want to deploy now? (Y/n) Y
```

### Deploying
```bash
PS D:\code\try-serverless> serverless

Creating a new serverless project

? What do you want to make? AWS - Node.js - HTTP API
? What do you want to call this project? greet

✔ Project successfully created in greet folder

? Register or Login to Serverless Framework Yes
Logging into the Serverless Framework via the browser
If your browser does not open automatically, please open this URL:
https://app.serverless.com?client=cli&transactionId=kYXs6ARC0OmvgxUdFfBSq

✔ You are now logged into the Serverless Framework


✔ Your project is ready to be deployed to Serverless Dashboard (org: "prawee", app: "greet")

? Do you want to deploy now? Yes

Deploying greet to stage dev (us-east-1)
✔ Serverless Framework's Observability features being set up on your AWS account (one-time set-up).
  An email will be sent upon completion, or view progress within the Dashboard:
  https://app.serverless.com/prawee/settings/integrations

✔ Service deployed to stack greet-dev (175s)

dashboard: https://app.serverless.com/prawee/apps/greet/greet/dev/us-east-1
endpoint: GET - https://umfo2xkq24.execute-api.us-east-1.amazonaws.com/
functions:
  api: greet-dev-api (204 kB)

What next?
Run these commands in the project directory:

serverless deploy    Deploy changes
serverless info      View deployed endpoints and resources
serverless invoke    Invoke deployed functions
serverless --help    Discover more commands
PS D:\code\try-serverless>
```

