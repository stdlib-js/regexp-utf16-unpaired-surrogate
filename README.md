<!--

@license Apache-2.0

Copyright (c) 2018 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->

# reUtf16UnpairedSurrogate

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> [Regular expression][mdn-regexp] to match an unpaired [UTF-16][utf-16] surrogate.



<section class="usage">

## Usage

<!-- eslint-disable id-length -->

To use in Observable,

```javascript
reUtf16UnpairedSurrogate = require( 'https://cdn.jsdelivr.net/gh/stdlib-js/regexp-utf16-unpaired-surrogate@umd/browser.js' )
```

To vendor stdlib functionality and avoid installing dependency trees for Node.js, you can use the UMD server build:

```javascript
var reUtf16UnpairedSurrogate = require( 'path/to/vendor/umd/regexp-utf16-unpaired-surrogate/index.js' )
```

To include the bundle in a webpage,

```html
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/regexp-utf16-unpaired-surrogate@umd/browser.js"></script>
```

If no recognized module system is present, access bundle contents via the global scope:

```html
<script type="text/javascript">
(function () {
    window.reUtf16UnpairedSurrogate;
})();
</script>
```

#### reUtf16UnpairedSurrogate()

Returns a [regular expression][mdn-regexp] to match an unpaired [UTF-16][utf-16] surrogate. 

<!-- eslint-disable id-length -->

```javascript
var RE_UTF16_UNPAIRED_SURROGATE = reUtf16UnpairedSurrogate();

var bool = RE_UTF16_UNPAIRED_SURROGATE.test( 'abc\uD800def' );
// returns true
```

#### reUtf16UnpairedSurrogate.REGEXP

[Regular expression][mdn-regexp] to match an unpaired [UTF-16][utf-16] surrogate. 

```javascript
var bool = reUtf16UnpairedSurrogate.REGEXP.test( 'abc\uD800def' );
// returns true
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint-disable id-length -->

<!-- eslint no-undef: "error" -->

```html
<!DOCTYPE html>
<html lang="en">
<body>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/regexp-utf16-unpaired-surrogate@umd/browser.js"></script>
<script type="text/javascript">
(function () {

var RE_UTF16_UNPAIRED_SURROGATE = reUtf16UnpairedSurrogate();

var bool = RE_UTF16_UNPAIRED_SURROGATE.test( '\uD800' );
// returns true

bool = RE_UTF16_UNPAIRED_SURROGATE.test( '\uDC00' );
// returns true

bool = RE_UTF16_UNPAIRED_SURROGATE.test( 'abc' );
// returns false

})();
</script>
</body>
</html>
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/regexp-utf16-surrogate-pair`][@stdlib/regexp/utf16-surrogate-pair]</span><span class="delimiter">: </span><span class="description">return a regular expression to match a UTF-16 surrogate pair.</span>

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2023. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/regexp-utf16-unpaired-surrogate.svg
[npm-url]: https://npmjs.org/package/@stdlib/regexp-utf16-unpaired-surrogate

[test-image]: https://github.com/stdlib-js/regexp-utf16-unpaired-surrogate/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/regexp-utf16-unpaired-surrogate/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/regexp-utf16-unpaired-surrogate/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/regexp-utf16-unpaired-surrogate?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/regexp-utf16-unpaired-surrogate.svg
[dependencies-url]: https://david-dm.org/stdlib-js/regexp-utf16-unpaired-surrogate/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/regexp-utf16-unpaired-surrogate/tree/deno
[umd-url]: https://github.com/stdlib-js/regexp-utf16-unpaired-surrogate/tree/umd
[esm-url]: https://github.com/stdlib-js/regexp-utf16-unpaired-surrogate/tree/esm
[branches-url]: https://github.com/stdlib-js/regexp-utf16-unpaired-surrogate/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/regexp-utf16-unpaired-surrogate/main/LICENSE

[mdn-regexp]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions

[utf-16]: https://en.wikipedia.org/wiki/UTF-16

<!-- <related-links> -->

[@stdlib/regexp/utf16-surrogate-pair]: https://github.com/stdlib-js/regexp-utf16-surrogate-pair/tree/umd

<!-- </related-links> -->

</section>

<!-- /.links -->
