# Hoist-Peers-Webpack-Resolve-Plugin

use hoisting dep's peerDependencies even though already existing in dep's node_modules

English | [简体中文](./README-zh_CN.md)

1. [Install](#Install)
2. [Usage](#Usage)

## Install

```bash
npm i hoist-peers-webpack-resolve-plugin --save-dev
```

## Usage

### using webpack.config.js

```js
// webpack.config.js

// ...
const { HoistPeersWebpackResolvePlugin } = require('hoist-peers-webpack-resolve-plugin');

module.exports = {
  // ...
  resolve: {
    // ...
    plugins: [
      // ...
      new HoistPeersWebpackResolvePlugin({ deps: ['your-npm-link-dep-name'] })
    ]
  },
  // ...
}
```
