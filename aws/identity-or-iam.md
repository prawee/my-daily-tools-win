# How to checking was i am 

## Recheck `caller` after configured
```bash
PS C:\> aws sts get-caller-identity
{
    "UserId": "AIDA******************",
    "Account": "14099*******",
    "Arn": "arn:aws:iam::14099*******:user/p*********"
}

PS C:\>
```

## Get identity with profile
```bash
PS C:\> aws sts get-caller-identity --profile staging
{
    "UserId": "AIDAS**********",
    "Account": "1956********",
    "Arn": "arn:aws:iam::1956*******:user/p********"
}

PS C:\>
```
