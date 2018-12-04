# koa-static

[![NPM version](https://img.shields.io/npm/v/@zcorky/koa-static.svg?style=flat)](https://www.npmjs.com/package/@zcorky/koa-static)
[![Coverage Status](https://img.shields.io/coveralls/zcorky/koa-static.svg?style=flat)](https://coveralls.io/r/zcorky/koa-static)
[![Dependencies](https://david-dm.org/@zcorky/koa-static/status.svg)](https://david-dm.org/@zcorky/koa-static)
[![Build Status](https://travis-ci.com/zcorky/koa-static.svg?branch=master)](https://travis-ci.com/zcorky/koa-static)
![license](https://img.shields.io/github/license/zcorky/koa-static.svg)
[![issues](https://img.shields.io/github/issues/zcorky/koa-static.svg)](https://github.com/zcorky/koa-static/issues)

> Simple OnError for Koa

### Install

```
$ npm install @zcorky/koa-static
```

### Usage

```javascript
// See more in test
import staticCache from '@zcorky/koa-static';

import * as Koa from 'koa';
const app = new Koa();

// fallback
app.use(staticCache('/static', {
  dir: path.join(__dirname, './public'),
}));

app.listen(8000, '0.0.0.0', () => {
  console.log('koa server start at port: 8000');
});
```

### Related
* [koa-static-cache](https://github.com/koajs/static-cache)
* [express.static/serve-static](https://github.com/expressjs/serve-static)