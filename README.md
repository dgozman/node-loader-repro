## Steps to reproduce

- Install Node.js v22.7.0.
- Run `node main.js`:

```
> node main.js
node:internal/assert:14
    throw new ERR_INTERNAL_ASSERTION(message);
    ^

Error [ERR_INTERNAL_ASSERTION]: This is caused by either a bug in Node.js or incorrect usage of Node.js internals.
Please open an issue with this stack trace at https://github.com/nodejs/node/issues

    at assert (node:internal/assert:14:11)
    at ModuleLoader.getModuleJobForRequire (node:internal/modules/esm/loader:329:5)
    at new ModuleJobSync (node:internal/modules/esm/module_job:313:34)
    at ModuleLoader.importSyncForRequire (node:internal/modules/esm/loader:314:11)
    at loadESMFromCJS (node:internal/modules/cjs/loader:1381:24)
    at Module._compile (node:internal/modules/cjs/loader:1503:5)
    at Module._extensions..js (node:internal/modules/cjs/loader:1691:10)
    at Module.load (node:internal/modules/cjs/loader:1317:32)
    at Module._load (node:internal/modules/cjs/loader:1127:12)
    at TracingChannel.traceSync (node:diagnostics_channel:315:14) {
  code: 'ERR_INTERNAL_ASSERTION'
}

Node.js v22.7.0
```
