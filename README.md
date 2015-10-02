compiLESS
=========

Compiles LESS files throughout a directory tree and exports them to a specific directory.


Usage
-----
Install required dependencies
```shell
$ npm install
```

Then in some file that is called upon app start (should only be called once):
```js
require("compiless")({
  "./src/less": "./public/css"
});
```

This will take any LESS files from the `assets/less` directory, compile them, and export them to the `public/css` directory.


Important notes
---------------
* Found directories will be recursivly searched.
* If a directory does not exist, it will be created.
* Previous files at a path **WILL** be overwritten


Running tests
-------------
Ensure you have mocha installed.

```shell
$ mocha
```