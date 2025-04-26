# How to build docker on windows with `cli-plugins`

## Required
- source code

## Build with `buildx`
```bash
PS D:\code\try-hono> docker buildx build -t prawee/hono:0.0.2 .
[+] Building 1.4s (10/10) FINISHED                                                                 docker:desktop-linux
 => [internal] load build definition from Dockerfile                                                               0.0s
 => => transferring dockerfile: 188B                                                                               0.0s
 => [internal] load metadata for docker.io/oven/bun:latest                                                         1.0s
 => [internal] load .dockerignore                                                                                  0.0s
 => => transferring context: 2B                                                                                    0.0s
 => [1/5] FROM docker.io/oven/bun:latest@sha256:420d7f4b99caadf1727ced361ae9455fbd175d54e3ec7ed698901fbf67cb2b1f   0.0s
 => => resolve docker.io/oven/bun:latest@sha256:420d7f4b99caadf1727ced361ae9455fbd175d54e3ec7ed698901fbf67cb2b1f   0.0s
 => [internal] load build context                                                                                  0.1s
 => => transferring context: 79.11kB                                                                               0.1s
 => CACHED [2/5] WORKDIR /app                                                                                      0.0s
 => CACHED [3/5] COPY . .                                                                                          0.0s
 => CACHED [4/5] RUN bun install                                                                                   0.0s
 => CACHED [5/5] RUN bun run build                                                                                 0.0s
 => exporting to image                                                                                             0.1s
 => => exporting layers                                                                                            0.0s
 => => exporting manifest sha256:da8ea54f1f760766539482f4c202cd6457101b94af92648188ab8124c4046d71                  0.0s
 => => exporting config sha256:e7d4b97284118e8e106b80c210f51a46beb0cfbe15c36ae020f053809e488987                    0.0s
 => => exporting attestation manifest sha256:1d5763c30bcf6f5ed3a16516cdb5a180ceab32c557860d9ccd2cc1c94a1022df      0.0s
 => => exporting manifest list sha256:902f859b4205e3669881b94ddb5791ec1fb87757a027e18ef58473c3a6491666             0.0s
 => => naming to docker.io/prawee/hono:0.0.2                                                                       0.0s
 => => unpacking to docker.io/prawee/hono:0.0.2                                                                    0.0s
```

## Image
```bash
PS D:\code\try-hono> docker images
REPOSITORY    TAG       IMAGE ID       CREATED         SIZE
prawee/hono   0.0.2     902f859b4205   2 minutes ago   386MB
prawee/hono   0.0.1     d26b35c4484e   2 minutes ago   386MB
```
