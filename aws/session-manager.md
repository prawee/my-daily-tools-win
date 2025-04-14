# How to using `Session Manager` of AWS

## Install plugin if nothing
```bash
PS C:\> scoop install extras/aws-session-manager-plugin
```

## Connect session with `RDS`
```bash
PS C:\> aws ssm start-session --target {{InstancesID}} --document-name AWS-StartPortForwardingSessionToRemoteHost --parameters host="{{InstanceName}}.xxxxx.ap-southeast-7.rds.amazonaws.com",portNumber="3306",localPortNumber="3306"
```