# µdomdiff

[![Coverage Status](https://coveralls.io/repos/github/WebReflection/udomdiff/badge.svg?branch=master)](https://coveralls.io/github/WebReflection/udomdiff?branch=master) [![Build Status](https://travis-ci.org/WebReflection/udomdiff.svg?branch=master)](https://travis-ci.org/WebReflection/udomdiff) [![License: ISC](https://img.shields.io/badge/License-ISC-yellow.svg)](https://opensource.org/licenses/ISC)

An essential version of [domdiff](https://github.com/WebReflection/domdiff#readme) for [µhtml](https://github.com/WebReflection/uhtml#readme).

#### Diffing Strategies:

  * common prefixes
  * common suffixes
  * skip same lists
  * add boundaries
  * remove boundaries
  * last fallback with a simplified Hunt Szymanski algorithm

### Signature

```js
futureNodes = udomdiff(
  parentNode,     // where changes happen
  currentNodes,   // Array of current items/nodes
  futureNodes,    // Array of future items/nodes (returned)
  get,            // a callback to retrieve the node
  before          // the anchored node to insertBefore
);
```

### How to import it:

  * via **CDN**, as global variable: `https://unpkg.com/udomdiff`
  * via **ESM**, as external module: `https://unpkg.com/udomdiff/esm/index.js`
  * via **CJS**: `const EventTarget = require('udomdiff').default;` <sup><sub>( or `require('udomdiff/cjs').default` )</sub></sup>
  * via bundlers/transpilers: `import udomdiff from 'udomdiff';` <sup><sub>( or `from 'udomdiff/esm'` )</sub></sup>
