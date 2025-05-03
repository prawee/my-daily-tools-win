# How to create model or schema with `Prisma`

## Info
Stand on your root project

## Let's go
```bash
cd prisma
nano prisma.schema
```

```bash
...
model User {
  id Int @id @default(autoincrement())
  username String
  password String
}
```

## Format first
```bash
npx prisma format
```
