
# regex-sort

 [![PayPal](https://img.shields.io/badge/%24-paypal-f39c12.svg)][paypal-donations] [![AMA](https://img.shields.io/badge/ask%20me-anything-1abc9c.svg)](https://github.com/IonicaBizau/ama) [![Version](https://img.shields.io/npm/v/regex-sort.svg)](https://www.npmjs.com/package/regex-sort) [![Downloads](https://img.shields.io/npm/dt/regex-sort.svg)](https://www.npmjs.com/package/regex-sort) [![Get help on Codementor](https://cdn.codementor.io/badges/get_help_github.svg)](https://www.codementor.io/johnnyb?utm_source=github&utm_medium=button&utm_term=johnnyb&utm_campaign=github)

> Sort an array of strings using regex patterns.

## :cloud: Installation

```sh
$ npm i --save regex-sort
```


## :clipboard: Example



```js
const regexSort = require("regex-sort");

let result = regexSort([
    "path/to/index.json",
    "path/to/foo.js",
    "path/to/index.min.js",
    "path/to/index.js"
], [
    /index\.(min\.)?js$/
  , /index\.json$/
]);

console.log(result);
// [ 'path/to/index.js',
//   'path/to/index.min.js',
//   'path/to/index.json',
//   'path/to/foo.js' ]
```

## :memo: Documentation


### `regexSort(list, patterns)`
Sort an array of strings using regex patterns.

#### Params
- **Array** `list`: An array of strings.
- **Array** `patterns`: An array of regular expressions used in sorting.

#### Return
- **Array** A new array containing the sorted elements.



## :yum: How to contribute
Have an idea? Found a bug? See [how to contribute][contributing].


## :scroll: License

[MIT][license] © [Ionică Bizău][website]

[paypal-donations]: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=RVXDDLKKLQRJW
[donate-now]: http://i.imgur.com/6cMbHOC.png

[license]: http://showalicense.com/?fullname=Ionic%C4%83%20Biz%C4%83u%20%3Cbizauionica%40gmail.com%3E%20(http%3A%2F%2Fionicabizau.net)&year=2016#license-mit
[website]: http://ionicabizau.net
[contributing]: /CONTRIBUTING.md
[docs]: /DOCUMENTATION.md
