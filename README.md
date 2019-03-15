# rtmcore-build

A helper to add tasks to gulp.

## Getting started

Install with:

```sh
npm install rtmcore-build
```

and use and require in your gulp file:

```javascript
var gulp = require('gulp');
var rtmcoreTasks = require('rtmcore-build');

rtmcoreTasks('submodule');
gulp.task('default', ['lint', 'test', 'browser', 'coverage']);
```

### Notes

* There's no default task to allow for each submodule to set up their own configuration
* If the module is node-only, avoid adding the browser tasks with:
```javascript
var rtmcoreTasks = require('rtmcore-build');
rtmcoreTasks('submodule', {skipBrowsers: true});
```

## Contributing

See [CONTRIBUTING.md](https://github.com/Raptor3um/rtmcore) on the main rtmcore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/Raptor3um/rtmcore/blob/master/LICENSE).

