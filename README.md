# MongoDemon
[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/indexzero/winston-mongodb?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

An experimental MongoDB 3.6 transport for [winston][0].

Current version supports only mongodb driver version 3.x.

## Motivation
`tldr;?`: To break the [winston][0] codebase into small modules that work
together.

The [winston][0] codebase has been growing significantly with contributions and
other logging transports. This is **awesome**. However, taking a ton of
additional dependencies just to do something simple like logging to the Console
and a File is overkill.  

## Usage
``` js
  var winston = require('winston');

  /**
   * Requiring `winston-mongodb` will expose
   * `winston.transports.MongoDB`
   */
  require('winston-mongodb');

  winston.add(winston.transports.MongoDB, options);
```

This MongoDB transport requires 'db' & 'dbName'.

[0]: https://github.com/flatiron/winston
