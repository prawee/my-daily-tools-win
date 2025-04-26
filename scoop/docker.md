# How to install `Docker Desktop` with scoop

## Searching
```bash
PS C:\> scoop search docker
Results from local buckets...

Name             Version         Source   Binaries
----             -------         ------   --------
docker-buildx    0.23.0          main
docker-compose   2.35.1          main
docker-machine   0.16.2          main
docker-pushrm    1.9.0           main
docker           28.1.1          main
lazydocker       0.24.1          main
dockercompletion 1.2704.0.241216 extras
gcloud           519.0.0         extras   docker-credential-gcloud.cmd
posh-docker      0.7.0           extras
docker-nightly   nightly         versions


PS C:\>
```

## Installation
```bash
PS C:\> scoop install docker
Installing 'docker' (28.1.1) [64bit] from 'main' bucket
docker-28.1.1.zip (40.0 MB) [=================================================================================] 100%
Checking hash of docker-28.1.1.zip ... ok.
Extracting docker-28.1.1.zip ... done.
Linking ~\scoop\apps\docker\current => ~\scoop\apps\docker\28.1.1
Creating shim for 'docker'.
Creating shim for 'dockerd'.
'docker' (28.1.1) was installed successfully!
Notes
-----
The 'dockerd' binary here only supports running Windows containers.
However it is possible to connect to existing Linux containers using the 'docker' binary
To register Docker as a service, run `dockerd --register-service`
Similarly, to unregister, run `dockerd --unregister-service`
PS C:\>
```

## Version
```bash
PS C:\> docker --version
Docker version 28.1.1, build 4eba377
PS C:\>
```
