# [Prestashop 1.7.x REST client](https://github.com/alexgenovese/prestashop-api-nodejs)


[![NPM version](https://img.shields.io/npm/v/prestashop-api-nodejs?style=flat-square)](https://www.npmjs.com/package/prestashop-api-nodejs)
[![NPM downloads](https://img.shields.io/npm/dm/prestashop-api-nodejs?style=flat-square)](https://www.npmjs.com/package/prestashop-api-nodejs)
[![NPM license](https://img.shields.io/npm/l/prestashop-api-nodejs?style=flat-square)](https://www.npmjs.com/package/prestashop-api-nodejs)
[![Travis](https://img.shields.io/travis/com/alexgenovese/prestashop-api-nodejs/master?style=flat-square)](https://travis-ci.com/alexgenovese/prestashop-api-nodejs.svg?branch=main)

This Node.js library enables JavaScript applications to communicate with Prestashop 1.7.x sites using their REST API.

**NOTE: the module is made up by base functions!**


## Installation

The library can be installed using the Npm package manager:

```
    npm install --save github:alexgenovese/prestashop-api-nodejs
```

## Usage

The code sample below shows the usage of the library:

```javascript
    var Prestashop = require('prestashop-api-nodejs');

    var options = {
          url: 'prestashop.local',
          key: '<Prestashop Token>'
    };
    var client = new Prestashop(options);
    await client.get({
          resource: 'customers',
          output_format: 'JSON',
          ws_key: '<Prestashop Token>'
        })
```
