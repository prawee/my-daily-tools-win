# How to push image to docker hub

After build finished if you want push to `Docker Hub`

## Validate image
```bash
PS D:\code\try-hono> docker images
REPOSITORY    TAG       IMAGE ID       CREATED         SIZE
prawee/hono   0.0.1     04d2dcef028f   3 minutes ago   386MB
```

## Pushing
```bash
PS D:\code\try-hono> docker image push prawee/hono:0.0.1
The push refers to repository [docker.io/prawee/hono]
23b7d26ef1d2: Pushed 
25fbe47460b0: Pushed 
afdf78891c33: Pushed 
4e61ef8b2d34: Pushed 
d4cb84934b16: Pushed 
e157f00fce11: Pushed 
f1c5a40681b5: Pushed 
6bdbd27ab659: Pushed 
f17eeda063b5: Pushed 
65a880e8f146: Pushed 
cfc955b51b8c: Pushed 
0.0.1: digest: sha256:04d2dcef028f1cc172cc313fbde6bbbd38b230594ccf65e78a857118ba663c08 size: 856
```

## Watch
open <https://hub.docker.com/repositories/{userId}>
