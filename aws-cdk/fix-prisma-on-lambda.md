# How to fix `Prisma` on Lambda stack

## Error with `Binary target`
```bash
{
    "errorType": "Runtime.UnhandledPromiseRejection",
    "errorMessage": "PrismaClientInitializationError: Prisma Client could not locate the Query Engine for runtime \"rhel-openssl-3.0.x\".\n\nThis happened because Prisma Client was generated for \"windows\", but the actual deployment required \"rhel-openssl-3.0.x\".\nAdd \"rhel-openssl-3.0.x\" to `binaryTargets` in the \"schema.prisma\" file and run `prisma generate` after saving it:\n\ngenerator client {\n  provider      = \"prisma-client-js\"\n  binaryTargets = [\"native\", \"rhel-openssl-3.0.x\"]\n}\n\nThe following locations have been searched:\n  /var/task/node_modules/.prisma/client\n  /var\n  D:\\code\\try-hono\\node_modules\\@prisma\\client\n  /.prisma/client\n  /tmp/prisma-engines",
    "reason": {
        "errorType": "PrismaClientInitializationError",
        "errorMessage": "Prisma Client could not locate the Query Engine for runtime \"rhel-openssl-3.0.x\".\n\nThis happened because Prisma Client was generated for \"windows\", but the actual deployment required \"rhel-openssl-3.0.x\".\nAdd \"rhel-openssl-3.0.x\" to `binaryTargets` in the \"schema.prisma\" file and run `prisma generate` after saving it:\n\ngenerator client {\n  provider      = \"prisma-client-js\"\n  binaryTargets = [\"native\", \"rhel-openssl-3.0.x\"]\n}\n\nThe following locations have been searched:\n  /var/task/node_modules/.prisma/client\n  /var\n  D:\\code\\try-hono\\node_modules\\@prisma\\client\n  /.prisma/client\n  /tmp/prisma-engines",
        "clientVersion": "6.7.0",
        "name": "PrismaClientInitializationError",
        "stack": [
            "PrismaClientInitializationError: Prisma Client could not locate the Query Engine for runtime \"rhel-openssl-3.0.x\".",
            "",
            "This happened because Prisma Client was generated for \"windows\", but the actual deployment required \"rhel-openssl-3.0.x\".",
            "Add \"rhel-openssl-3.0.x\" to `binaryTargets` in the \"schema.prisma\" file and run `prisma generate` after saving it:",
            "",
            "generator client {",
            "  provider      = \"prisma-client-js\"",
            "  binaryTargets = [\"native\", \"rhel-openssl-3.0.x\"]",
            "}",
            "",
            "The following locations have been searched:",
            "  /var/task/node_modules/.prisma/client",
            "  /var",
            "  D:\\code\\try-hono\\node_modules\\@prisma\\client",
            "  /.prisma/client",
            "  /tmp/prisma-engines",
            "    at hl (/var/task/index.js:4023:77)",
            "    at async Object.loadLibrary (/var/task/index.js:4648:31)",
            "    at async Qr.loadEngine (/var/task/index.js:4779:58)",
            "    at async Qr.instantiateLibrary (/var/task/index.js:4758:72)"
        ]
    },
    "promise": {},
    "stack": [
        "Runtime.UnhandledPromiseRejection: PrismaClientInitializationError: Prisma Client could not locate the Query Engine for runtime \"rhel-openssl-3.0.x\".",
        "",
        "This happened because Prisma Client was generated for \"windows\", but the actual deployment required \"rhel-openssl-3.0.x\".",
        "Add \"rhel-openssl-3.0.x\" to `binaryTargets` in the \"schema.prisma\" file and run `prisma generate` after saving it:",
        "",
        "generator client {",
        "  provider      = \"prisma-client-js\"",
        "  binaryTargets = [\"native\", \"rhel-openssl-3.0.x\"]",
        "}",
        "",
        "The following locations have been searched:",
        "  /var/task/node_modules/.prisma/client",
        "  /var",
        "  D:\\code\\try-hono\\node_modules\\@prisma\\client",
        "  /.prisma/client",
        "  /tmp/prisma-engines",
        "    at process.<anonymous> (file:///var/runtime/index.mjs:1276:17)",
        "    at process.emit (node:events:518:28)",
        "    at emitUnhandledRejection (node:internal/process/promises:250:13)",
        "    at throwUnhandledRejectionsMode (node:internal/process/promises:385:19)",
        "    at processPromiseRejections (node:internal/process/promises:470:17)",
        "    at process.processTicksAndRejections (node:internal/process/task_queues:96:32)"
    ]
}
```

### Fix 
```bash
nano prisma/schema.prisma
```
```bash
generator client {
  ...
  binaryTargets = ["native", "rhel-openssl-3.0.x"]
}
```
```bash
npx prisma generate
```



## Reference
<https://www.prisma.io/docs/orm/prisma-client/deployment/serverless/deploy-to-aws-lambda>
