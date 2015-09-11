# Index
1. [Intro](#intro)
1. [Strings](#strings)
1. [Numbers](#numbers)
1. [Arrays](#arrays)
1. [Objects](#objects)
1. [RegExp](#regexp)
1. [Functions](#functions)
1. [Basic Conditionals](#basic-conditionals) (`if`, `else if`, etc)
1. [Loops](#loops)
1. [Scoping](#scoping)
1. [Variables](#variables)
1. [Other](#other)

# Numbers
# Arrays
# Objects
# RegExp
# Functions
# Basic Conditionals

# Loops
## Statements
### Conditional
#### `for`
+ `for`
  + Use it when you know the start and end of a loop.
+ `for...in`
  + Enumerate over an object.
  + Discouraged for arrays. Use `for...of` instead.
+ `for...of`
  + Enumerate arrays and objects.
+ ~~`for each...in`~~
  + Don't use it. It's obsolete. Use `for...of` instead.

#### `while`
+ `while`
  + Use it when you know the start but not the end of a loop.
+ `do...while`
  + Use it when you want to to manipulate the iterator in the loop itself.
  + Executes once before it loops.

#### `Array.prototype.forEach`
+ `.forEach`
  + Use it when you want to get each item and index in an array.
  + It follows `.forEach(callback[, thisArg])`, where `thisArg` would be represented as `this` in the callback.
  + The callback contains the arguments `currentValue, index, array`.

### Operational
+ `label`
  + Names the loop so you can hop to it with the `condition` statement.
+ `break`
  + Stops a loop.
+ `continue`
  + Moves to the next iteration.

# Variables
# Other

---

# Built-in Objects

## Index
1. [String](#string)
1. [RegExp](#RegExp)

## Legend
       | Description
:----: | ------------------------
✅ | Safe to use
❎ | Safe to use but not recommended
🚧 | Some support
❌ | Deprecated
❓ | Non-standard

## String
### Properties
#### ES1
       | String.*property* | Info
:----: | ----------------- | -----------------
✅ | `length` | 🔹 Returns the length of a string.
✅ | `prototype` | 🔹 Represents the string prototype object.

### Methods
#### ES1
       | String.prototype.*method* | Info
:----: | ----------------- | -----------------
❎ | ~~`fromCharCode()`~~ | 🔹 Returns a string from a sequence of Unicode values. <br> 🔹 Cannot return all Unicode characters. <br> 🔹 Use `String.fromCodePoint()` instead.
✅ | `charAt()`
✅ | `charCodeAt()`
✅ | `indexOf()`
✅ | `lastIndexOf()`
❎ | ~~`substring()`~~ | 🔹 Returns a section of a string from a start and an optional end index. <br> 🔹 Almost identical to `String.prototype.slice()`, use it instead.
✅ | `toLowerCase()`
✅ | `toUpperCase()`
✅ | `valueOf()` | 🔹 Returns the primitive value of a String object.

#### ES3
       | String.prototype.*method* | Info
:----: | ----------------- | -----------------
✅ | `concat()`
✅ | `localeCompare()`
✅ | `match()`
✅ | `replace()`
✅ | `search()`
✅ | `slice()`
✅ | `split()` | 🔹 Returns a section of a string from a start and an optional end index.
✅ | `substr()`
✅ | `toLocaleLowerCase()`
✅ | `toLocaleUpperCase()`
✅ | `toString()`

#### ES5.1
       | String.prototype.*method* | Info
:----: | ----------------- | -----------------
✅ | `trim()` | 🔹 Removes whitespace from both ends of a string.

#### ES6

##### Not HTML
       | String.prototype.*method* | Info
:----: | ----------------- | -----------------
🚧 | `fromCodePoint()` | 🔹 Returns a string from a sequence of code points.
🚧 | `codePointAt()`
🚧 | `endsWidth()`
🚧 | `includes()`
🚧 | `normalize()`
🚧 | `repeat()`
🚧 | `startsWith()`
🚧 | `[@@iterator]()`
🚧 | `raw()`

##### HTML Wrappers
       | String.prototype.*method* | Info
:----: | ----------------- | -----------------
✅ | `anchor()`
❌ | ~~`big()`~~
❌ | ~~`blink()`~~
❌ | ~~`bold()`~~
❌ | ~~`fixed()`~~
❌ | ~~`fontcolor()`~~
❌ | ~~`fontsize()`~~
❌ | ~~`italics()`~~
✅ | `link()`
❌ | ~~`small()`~~
❌ | ~~`strike()`~~
❌ | ~~`stub()`~~
❌ | ~~`sup()`~~

#### Non-standard
       | String.prototype.*method* | Info
:----: | ----------------- | -----------------
❓ | ~~`quote()`~~
❓ | ~~`toSource()`~~
❓ | ~~`trimLeft()`~~
❓ | ~~`trimRight()`~~

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
