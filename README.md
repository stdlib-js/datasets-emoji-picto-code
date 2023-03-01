<!--

@license Apache-2.0

Copyright (c) 2019 The Stdlib Authors.

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

# Emoji Pictographs and Codes

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Map emoji pictographs to codes.

<section class="installation">

## Installation

```bash
npm install @stdlib/datasets-emoji-picto-code
```

Alternatively,

-   To load the package in a website via a `script` tag without installation and bundlers, use the [ES Module][es-module] available on the [`esm` branch][esm-url].
-   If you are using Deno, visit the [`deno` branch][deno-url].
-   For use in Observable, or in browser/node environments, use the [Universal Module Definition (UMD)][umd] build available on the [`umd` branch][umd-url].
-   To use as a general utility for the command line, install the corresponding [CLI package][cli-section] globally.

The [branches.md][branches-url] file summarizes the available branches and displays a diagram illustrating their relationships.

</section>

<section class="usage">

## Usage

```javascript
var table = require( '@stdlib/datasets-emoji-picto-code' );
```

#### table()

Returns an object mapping emoji pictographs to codes.

```javascript
var t = table();
// returns {...}

var p = t[ '😄' ];
// returns [ ':smile:' ]

p = t[ '🦄' ];
// returns [ ':unicorn:' ]
```

</section>

<!-- /.usage -->

<section class="notes">

## Notes

-   Some emoji pictographs may have **multiple** applicable codes.

</section>

<!-- ./notes -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```javascript
var objectKeys = require( '@stdlib/utils-keys' );
var table = require( '@stdlib/datasets-emoji-picto-code' );

var picto;
var tbl;
var i;

// Get the data:
tbl = table();

// Get the emoji pictographs:
picto = objectKeys( tbl );

// Print out all the corresponding codes...
for ( i = 0; i < picto.length; i++ ) {
    console.log( picto[ i ] + ' => ' + tbl[ picto[ i ] ] );
}
```

</section>

<!-- /.examples -->

* * *

<section class="cli">

## CLI

<section class="installation">

## Installation

To use as a general utility, install the CLI package globally

```bash
npm install -g @stdlib/datasets-emoji-picto-code-cli
```

</section>

<!-- CLI usage documentation. -->

<section class="usage">

### Usage

```text
Usage: emoji-picto-code [options]

Options:

  -h,    --help                Print this message.
  -V,    --version             Print the package version.
```

</section>

<!-- /.usage -->

<section class="notes">

### Notes

-   Data is written to `stdout` as comma-separated values ([CSV][csv]), where the first line is a header line.

</section>

<!-- /.notes -->

<section class="examples">

### Examples

```bash
$ emoji-picto-code
emoji,code
...
```

</section>

<!-- /.examples -->

</section>

<!-- /.cli -->

<!-- <license> -->

## License

The data files (databases) are licensed under an [Open Data Commons Public Domain Dedication & License 1.0][pddl-1.0] and their contents are licensed under [Creative Commons Zero v1.0 Universal][cc0]. The software is licensed under [Apache License, Version 2.0][apache-license].

<!-- </license> -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/datasets-emoji`][@stdlib/datasets/emoji]</span><span class="delimiter">: </span><span class="description">emoji.</span>
-   <span class="package-name">[`@stdlib/datasets-emoji-code-picto`][@stdlib/datasets/emoji-code-picto]</span><span class="delimiter">: </span><span class="description">emoji codes and pictographs.</span>

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

## Copyright

Copyright &copy; 2016-2023. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/datasets-emoji-picto-code.svg
[npm-url]: https://npmjs.org/package/@stdlib/datasets-emoji-picto-code

[test-image]: https://github.com/stdlib-js/datasets-emoji-picto-code/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/datasets-emoji-picto-code/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/datasets-emoji-picto-code/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/datasets-emoji-picto-code?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/datasets-emoji-picto-code.svg
[dependencies-url]: https://david-dm.org/stdlib-js/datasets-emoji-picto-code/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[cli-section]: https://github.com/stdlib-js/datasets-emoji-picto-code#cli
[cli-url]: https://github.com/stdlib-js/datasets-emoji-picto-code/tree/cli
[@stdlib/datasets-emoji-picto-code]: https://github.com/stdlib-js/datasets-emoji-picto-code/tree/main

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/datasets-emoji-picto-code/tree/deno
[umd-url]: https://github.com/stdlib-js/datasets-emoji-picto-code/tree/umd
[esm-url]: https://github.com/stdlib-js/datasets-emoji-picto-code/tree/esm
[branches-url]: https://github.com/stdlib-js/datasets-emoji-picto-code/blob/main/branches.md

[pddl-1.0]: http://opendatacommons.org/licenses/pddl/1.0/

[cc0]: https://creativecommons.org/publicdomain/zero/1.0

[apache-license]: https://www.apache.org/licenses/LICENSE-2.0

[csv]: https://tools.ietf.org/html/rfc4180

<!-- <related-links> -->

[@stdlib/datasets/emoji]: https://github.com/stdlib-js/datasets-emoji

[@stdlib/datasets/emoji-code-picto]: https://github.com/stdlib-js/datasets-emoji-code-picto

<!-- </related-links> -->

</section>

<!-- /.links -->
