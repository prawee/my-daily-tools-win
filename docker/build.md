# How to build docker on windows

## Required
- source code

## Build
```bash
PS D:\code\try-hono> docker build -t prawee/hono:0.0.1 .
[+] Building 15.9s (10/10) FINISHED                                                                                                                                                         docker:desktop-linux
 => [internal] load build definition from Dockerfile                                                                                                                                                        0.0s
 => => transferring dockerfile: 188B                                                                                                                                                                        0.0s
 => [internal] load metadata for docker.io/oven/bun:latest                                                                                                                                                  1.0s
 => [internal] load .dockerignore                                                                                                                                                                           0.0s
 => => transferring context: 2B                                                                                                                                                                             0.0s
 => [1/5] FROM docker.io/oven/bun:latest@sha256:420d7f4b99caadf1727ced361ae9455fbd175d54e3ec7ed698901fbf67cb2b1f                                                                                            8.0s
 => => resolve docker.io/oven/bun:latest@sha256:420d7f4b99caadf1727ced361ae9455fbd175d54e3ec7ed698901fbf67cb2b1f                                                                                            0.0s
 => => sha256:f1c5a40681b5a8529ae107d2c403cd5d6ba7eb50f1c592683ade38613a05ed69 135B / 135B                                                                                                                  0.6s
 => => sha256:65a880e8f1464ef268cdd3a0e6e1afb2f59b8cfa29fdca9772e8a162399aa544 3.40kB / 3.40kB                                                                                                              0.9s
 => => sha256:25fbe47460b016fc4da5c168cb608b601db4490cef7312eb79983317a1e729dc 38.92MB / 38.92MB                                                                                                            5.0s
 => => sha256:4e61ef8b2d34b240c39cb3abf7a3f22c67de1171e82713d5cec4ed3ec9276474 184B / 184B                                                                                                                  1.1s
 => => sha256:e157f00fce11303b9c9cb588a4a7795caae6f59c544e46642385bf24ff7f6c3a 296B / 296B                                                                                                                  0.7s
 => => sha256:23b7d26ef1d294256da0d70ce374277b9aab5ca683015073316005cb63d33849 48.49MB / 48.49MB                                                                                                            4.3s
 => => extracting sha256:23b7d26ef1d294256da0d70ce374277b9aab5ca683015073316005cb63d33849                                                                                                                   1.9s
 => => extracting sha256:e157f00fce11303b9c9cb588a4a7795caae6f59c544e46642385bf24ff7f6c3a                                                                                                                   0.0s
 => => extracting sha256:25fbe47460b016fc4da5c168cb608b601db4490cef7312eb79983317a1e729dc                                                                                                                   0.6s
 => => extracting sha256:4e61ef8b2d34b240c39cb3abf7a3f22c67de1171e82713d5cec4ed3ec9276474                                                                                                                   0.0s
 => => extracting sha256:65a880e8f1464ef268cdd3a0e6e1afb2f59b8cfa29fdca9772e8a162399aa544                                                                                                                   0.0s
 => => extracting sha256:f1c5a40681b5a8529ae107d2c403cd5d6ba7eb50f1c592683ade38613a05ed69                                                                                                                   0.0s
 => [internal] load build context                                                                                                                                                                           0.2s
 => => transferring context: 78.48kB                                                                                                                                                                        0.1s
 => [2/5] WORKDIR /app                                                                                                                                                                                      0.3s
 => [3/5] COPY . .                                                                                                                                                                                          0.6s
 => [4/5] RUN bun install                                                                                                                                                                                   1.1s
 => [5/5] RUN bun run build                                                                                                                                                                                 2.2s
 => exporting to image                                                                                                                                                                                      2.6s 
 => => exporting layers                                                                                                                                                                                     1.8s 
 => => exporting manifest sha256:7b05011095af39fa790d983edb4ee731e019e7bbd0a8e0100c6cf458eb91aea0                                                                                                           0.0s
 => => exporting config sha256:abf77ea1eecfcf95b9cd9f88acd2b079c847a998158e1c9ec724ad7db3bc8385                                                                                                             0.0s
 => => exporting attestation manifest sha256:8f66b76424f08b9a27d6f4d97ae908a52b9a9451640ab5cab8d6a9c3e3fbc6b9                                                                                               0.0s
 => => exporting manifest list sha256:1e96837bde55daaf8e74c9add7ee2ab974a949ad9b225ce6014d1964412cc0ba                                                                                                      0.0s
 => => naming to docker.io/prawee/hono:0.0.1                                                                                                                                                                0.0s
 => => unpacking to docker.io/prawee/hono:0.0.1 
```

## Result with `docker images`
```bash
PS D:\code\try-hono> docker images
REPOSITORY    TAG       IMAGE ID       CREATED         SIZE
prawee/hono   0.0.1     1e96837bde55   8 seconds ago   386MB
```
