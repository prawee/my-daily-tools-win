# How to describe instances

## Finding instance is running with tag name
```bash
PS C:\> aws ec2 describe-instances --filter "Name=tag:Name,Values={{Instance Name}}" --query "Reservations[].Instances[?State.name == 'running'].InstanceId[]" --output text

or 

PS C:\> aws ec2 describe-instances --filter "Name=tag:Name,Values={{Instance Name}}" --output json
```

## Start session
```bash
PS C:\> aws ssm start-session --target {{InstancesID}} --document-name AWS-StartPortForwardingSessionToRemoteHost --parameters host="{{InstanceName}}.xxxxx.ap-southeast-7.rds.amazonaws.com",portNumber="3306",localPortNumber="3306"
```

### Error
```bash
SessionManagerPlugin is not found. Please refer to SessionManager Documentation here: http://docs.aws.amazon.com/console/systems-manager/session-manager-plugin-not-found
PS C:\>
```

### How to fix
```bash
PS C:\> scoop search aws
Results from local buckets...

Name                       Version   Source Binaries
----                       -------   ------ --------
aws-amplify                13.0.0    main
aws-copilot                1.34.1    main
aws-ecs                    1.21.0    main
aws-iam-authenticator      0.6.31    main
aws-nuke                   2.25.0    main
aws-sam-cli                1.137.1   main
aws-vault                  7.2.0     main
aws                        2.26.1    main
awsqueue                   0.0.8     main
awsSts                     0.9.1     main
saml2aws                   2.36.19   main
aws-nosql-workbench        3.13.5    extras
aws-session-manager-plugin 1.2.707.0 extras
claws-mail                 4.3.0-1   extras
wireshark                  4.4.5     extras rawshark.exe
```

```bash
PS C:\> scoop install extras/aws-session-manager-plugin
Updating Scoop...
WARN  Uncommitted changes detected. Update aborted.
Updating Buckets...
```

```bash
Installing 'dark' (3.14) [64bit] from 'main' bucket
dark-3.14.zip (5.0 MB) [======================================================================================] 100%
Checking hash of dark-3.14.zip ... ok.
Extracting dark-3.14.zip ... done.
Linking ~\scoop\apps\dark\current => ~\scoop\apps\dark\3.14
Creating shim for 'dark'.
'dark' (3.14) was installed successfully!
Installing 'aws-session-manager-plugin' (1.2.707.0) [64bit] from 'extras' bucket
SessionManagerPluginSetup.exe (8.0 MB) [======================================================================] 100%
Checking hash of SessionManagerPluginSetup.exe ... ok.
Running installer script...done.
Linking ~\scoop\apps\aws-session-manager-plugin\current => ~\scoop\apps\aws-session-manager-plugin\1.2.707.0
Creating shim for 'session-manager-plugin'.
'aws-session-manager-plugin' (1.2.707.0) was installed successfully!

PS C:\>
```

## Try it again
```bash
PS C:\> aws ssm start-session --target {{InstancesID}} --document-name AWS-StartPortForwardingSessionToRemoteHost --parameters host="{{InstanceName}}.xxxxx.ap-southeast-7.rds.amazonaws.com",portNumber="3306",localPortNumber="3306"
```

```bash
Starting session with SessionId: pxxxx.won-gzgpsxxxxxxxxxxxxxxxxxxxxxxx
Port 3306 opened for sessionId pxxxx.won-gzgpsxxxxxxxxxxxxxxxxxxxxxxx.
Waiting for connections...
Connection accepted for session [pxxxx.won-gzgpsxxxxxxxxxxxxxxxxxxxxxxx]
```

## Test to connect
```bash
PS C:\> mysql -h 127.0.0.1 -P 3306 -u {{user_name}} -D {{db_name}} -p
Enter password: *************
Welcome to the MariaDB monitor.  Commands end with ; or \g.
Your MySQL connection id is 12639
Server version: 8.0.40 Source distribution

Copyright (c) 2000, 2018, Oracle, MariaDB Corporation Ab and others.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

MySQL [highsum_db]>
```