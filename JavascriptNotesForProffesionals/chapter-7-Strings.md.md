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
- `String.fromCharCode` method:
```js
String.fromCharCode(104,101,108,108,111) //"hello"
```
- Creating a String object using `new` keyword is allowed, but is not recommended:
```js
var objectString = new String("Yes, I am a String object");
typeof objectString;//"object"
typeof objectString.valueOf();//"string"
```
#### Concatenating Strings:

- using `+` operator:
```js
var foo = "Foo";
var bar = "Bar";
var s="string";
var n=44;
var boolean=true;
console.log(foo+bar+s+n+boolean); // FooBarstring44true
```
- Using template literals (backticks) `hello`:
```js
var place=`World`;
var greet=`Hello ${place}!`; // "Hello World!"
```
- Use `String.raw` to get backslashes to be in the string without modification.
```js
`a\\b` // = a\b
String.raw`a\\b` // = a\\b
```
### Section 7.2: Reverse String:
The most "popular" way of reversing a string in JavaScript is:
```js
function reverseString(str) {
 return str.split('').reverse().join('');
}
reverseString('string');
 // "gnirts"
```


<!--stackedit_data:
eyJoaXN0b3J5IjpbMTgxNDAxNzYxXX0=
-->