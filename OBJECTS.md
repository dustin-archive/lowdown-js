# Built-in Objects

## Index
1. [String](#string)
1. [RegExp](#RegExp)

## Legend
|        | Description
| :----: | ------------------------
| ✅ | Safe to use
| ❎ | Safe to use but not recommended
| 🚧 | Some support
| ❌ | Deprecated
| ❓ | Non-standard

## String
### Properties
#### ES1
|        | String.*property* | Info
| :----: | ----------------- | -----------------
| ✅ | `length` | • Returns the length of a string.
| ✅ | `prototype` | • Represents the string prototype object.

### Methods
#### ES1
|        | String.prototype.*method()* | Info
| :----: | ----------------- | -----------------
| ❎ | ~~`fromCharCode()`~~ | • Returns a string from a sequence of Unicode values. <br> • Cannot return all Unicode characters. <br> • Use `String.fromCodePoint()` instead.
| ✅ | `charAt()`
| ✅ | `charCodeAt()`
| ✅ | `indexOf()` | • Returns the index of the first matching occurrence of the argument in a string or array.
| ✅ | `lastIndexOf()`
| ❎ | ~~`substring()`~~ | • Returns a section of a string from a start and an optional length of section. <br> • Doesn't handle negative numbers. <br> • Almost identical to `String.prototype.slice()`, use it instead.
| ✅ | `toLowerCase()`
| ✅ | `toUpperCase()`
| ✅ | `valueOf()` | • Returns the primitive value of a String object.

#### ES3
|        | String.prototype.*method()* | Info
| :----: | ----------------- | -----------------
| ✅ | `concat()` | • Returns a new array from the array it's called and the array or value from the argument.
| ✅ | `localeCompare()`
| ✅ | `match()`
| ✅ | `replace()`
| ✅ | `search()`
| ✅ | `slice()` | • Returns a section of a string from a start and an optional end index.
| ✅ | `split()` | • Returns an array from a string using any string of characters as a delimiter.
| ✅ | `substr()`
| ✅ | `toLocaleLowerCase()`
| ✅ | `toLocaleUpperCase()`
| ✅ | `toString()` | • Returns a string from any other datatype.

#### ES5.1
|        | String.prototype.*method()* | Info
| :----: | ----------------- | -----------------
| ✅ | `trim()` | • Returns a string with whitespace removed from both ends.

#### ES6

##### Not HTML
|        | String.prototype.*method()* | Info
| :----: | ----------------- | -----------------
| 🚧 | `fromCodePoint()` | • Returns a string from a sequence of code points.
| 🚧 | `codePointAt()`
| 🚧 | `endsWidth()`
| 🚧 | `includes()`
| 🚧 | `normalize()`
| 🚧 | `repeat()`
| 🚧 | `startsWith()`
| 🚧 | `[@@iterator]()`
| 🚧 | `raw()`

##### HTML Wrappers
|        | String.prototype.*method()* | Info
| :----: | ----------------- | -----------------
| ✅ | `anchor()`
| ❌ | ~~`big()`~~
| ❌ | ~~`blink()`~~
| ❌ | ~~`bold()`~~
| ❌ | ~~`fixed()`~~
| ❌ | ~~`fontcolor()`~~
| ❌ | ~~`fontsize()`~~
| ❌ | ~~`italics()`~~
| ✅ | `link()`
| ❌ | ~~`small()`~~
| ❌ | ~~`strike()`~~
| ❌ | ~~`stub()`~~
| ❌ | ~~`sup()`~~

#### Non-standard
|        | String.prototype.*method()* | Info
| :----: | ----------------- | -----------------
| ❓ | ~~`quote()`~~
| ❓ | ~~`toSource()`~~
| ❓ | ~~`trimLeft()`~~
| ❓ | ~~`trimRight()`~~

## RegExp
### Properties
+ `RegExp.$1-$9`
+ `RegExp.input ($_)`
+ `RegExp.lastIndex`
+ `RegExp.lastMatch ($&)`
+ `RegExp.lastParen ($+)`
+ `RegExp.lastContext ($`)`
+ `RegExp.prototype`
+ `RegExp.prototype.flags`
+ `RegExp.prototype.global`
+ `RegExp.prototype.ignoreCase`
+ `RegExp.prototype.multiline`
+ `RegExp.prototype.source`
+ `RegExp.prototype.sticky`
+ `RegExp.prototype.unicode`
+ `RegExp.prototype.rightContext ($')`

### Methods
+ `RegExp.prototype.compile()`
+ `RegExp.prototype.exec()`
+ `RegExp.prototype.test()`
+ `RegExp.prototype.toSource()`
+ `RegExp.prototype.toString()`

# Unorganized
|        | ? | Info
| :----: | ----------------- | -----------------
|  | ?.innerHtml | • Gets or sets the HTML from or to an element.
