---
title: "JSON-RPC"
---

# JSON-RPC

::: tip
You can find the source code of this package at [packages/core-json-rpc](https://github.com/ArkEcosystem/core/tree/develop/packages/core-json-rpc).
:::

## Installation

```bash
yarn add @arkecosystem/core-json-rpc
```

## Configuration

```js
module.exports = {
  enabled: process.env.ARK_JSON_RPC_ENABLED,
  host: process.env.ARK_JSON_RPC_HOST || '0.0.0.0',
  port: process.env.ARK_JSON_RPC_PORT || 8080,
  allowRemote: false,
  whitelist: ['127.0.0.1', '::ffff:127.0.0.1'],
  database: {
    uri: process.env.ARK_JSON_RPC_DATABASE || `sqlite://${process.env.ARK_PATH_DATA}/database/json-rpc.sqlite`,
    options: {},
  },
}

```
