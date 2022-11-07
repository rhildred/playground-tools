<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) > [php-wasm-browser](./php-wasm-browser.md) > [setURLScope](./php-wasm-browser.seturlscope.md)

## setURLScope() function
setURLScope<!-- -->(<!-- -->url<!-- -->: [URL](https://developer.mozilla.org/en-US/docs/Web/API/URL)<!-- -->|[string](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html#the-primitives-string-number-and-boolean)<!-- -->, scope<!-- -->: [string](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html#the-primitives-string-number-and-boolean)<!-- -->)<!-- -->: [URL](https://developer.mozilla.org/en-US/docs/Web/API/URL)

* `url` – The URL to scope.
* `scope` – The scope value.
* Returns: A new URL with the scope information in it.


Returns a new URL with the requested scope information.

## Example

```js
setURLScope(new URL('http://localhost/index.php'), '96253');
// URL('http://localhost/scope:96253/index.php')

setURLScope(new URL('http://localhost/scope:96253/index.php'), '12345');
// URL('http://localhost/scope:12345/index.php')

setURLScope(new URL('http://localhost/index.php'), null);
// URL('http://localhost/index.php')
```
