# How to configure of AWS

```bash
PS C:\> aws configure
```
```
AWS Access Key ID [None]: ****
AWS Secret Access Key [None]: ****
Default region name [None]: ap-southeast-7
Default output format [None]: json
```

## List profile
```bash
PS C:\> aws configure list-profiles
default
```
```
[default]
output = json
region = ap-southeast-1
```

## Create more profile
```bash
PS C:\> aws configure --profile staging
```
```
PS C:\> aws configure --profile staging
AWS Access Key ID [None]: ****
AWS Secret Access Key [None]: ****
Default region name [None]: ap-southeast-1
Default output format [None]: json
```

## List again
```bash
PS C:\> aws configure list-profiles
default
staging
```

## Example of profile
- default
- staging
- production
