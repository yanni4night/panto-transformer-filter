# panto-transformer-fitler
[![NPM version][npm-image]][npm-url] [![Downloads][downloads-image]][npm-url] [![Dependency status][david-dm-image]][david-dm-url] [![Dev Dependency status][david-dm-dev-image]][david-dm-dev-url]

Filter transformer for panto.

```
panto.loadTransformer('filter');

panto.pick('**/*').(panto.filter({
    pattern: [/.js$/, filename => {
        return filename[0] === 'a';
    }, 'src/**/*']
})).(panto.read()).end();
```

## options
 - pattern: array|regexp|string|function

[npm-url]: https://npmjs.org/package/panto-transformer-filter
[downloads-image]: http://img.shields.io/npm/dm/panto-transformer-filter.svg
[npm-image]: http://img.shields.io/npm/v/panto-transformer-filter.svg
[david-dm-url]:https://david-dm.org/pantojs/panto-transformer-filter
[david-dm-image]:https://david-dm.org/pantojs/panto-transformer-filter.svg
[david-dm-dev-url]:https://david-dm.org/pantojs/panto-transformer-filter#info=devDependencies
[david-dm-dev-image]:https://david-dm.org/pantojs/panto-transformer-filter/dev-status.svg