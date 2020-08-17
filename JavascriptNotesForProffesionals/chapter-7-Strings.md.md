### Section 7.1 Basic
Strings in JavaScript can be enclosed in Single quotes 'hello', Double quotes "Hello" and (from ES2015, ES6) in Template Literals (backticks) \`hello\`.

Strings can be created from other types using 

- the `String()` function.
```js
var intString = String(32); // "32"
var booleanString = String(true); // "true"
var nullString = String(null); // "null"
```
- `toString`  to convert Numbers, Booleans or Objects to Strings:
```js
var intString = (5232).toString(); // "5232"
var booleanString = (false).toString(); // "false"
var objString = ({}).toString(); // "[object Object]"
```

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTIwNTI2MzI4MjNdfQ==
-->