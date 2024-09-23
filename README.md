# practice-monorepo-pnpm-turborepo

## Build
```
# Build from root
pnpm --filter lib-a build
pnpm --filter lib-b build # dependency lib-a -> lib-b
pnpm --filter lib-b x # run
# Build from each dir
cd packages/lib-a && pnpm build && cd ../..
cd packages/lib-b && pnpm build && cd ../..
cd packages/lib-b && pnpm x && cd ../..
```
