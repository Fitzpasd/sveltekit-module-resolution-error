# ERR_MODULE_NOT_FOUND repro

Steps taken to create this repro:

1. `npm create svelte@latest`
2. `npm i`
3. `npm i @typedorm/core @typedorm/common reflect-metadata --save-dev`
4. Created the `hooks.server.ts` file with `@typedorm/core` import
5. `npm run build`

Error given:

```
Error [ERR_MODULE_NOT_FOUND]: Cannot find module '/home/<me>/repos/sveltekit-module-resolution-error/node_modules/@typedorm/common/esm/public-api' imported from /home/<me>/repos/sveltekit-module-resolution-error/node_modules/@typedorm/common/esm/index.js
```
