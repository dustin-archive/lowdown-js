TLDR.js
=======
Unofficial opinionated TL;DR of JavaScript.

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
+ <s>`for each...in`</s>
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
+ ✅ Safe to use
+ ❎ Safe to use but not recommended
+ 🚧 Some support
+ ❌ Deprecated
+ ❓ Non-standard

## String
### Properties
#### ES1
+ ✅ `String.length`
  + Returns the length of a string.  
+ ✅ `String.prototype`

### Methods
#### ES1
+ ❎ <s>`String.prototype.fromCharCode()`</s>
  + Returns a string from a sequence of Unicode values.
  + Cannot return all Unicode characters. Use `String.fromCodePoint()` instead.
+ ✅ `String.prototype.charAt()`
+ ✅ `String.prototype.charCodeAt()`
+ ✅ `String.prototype.indexOf()`
+ ✅ `String.prototype.lastIndexOf()`
+ ❎ <s>`String.prototype.substring()`</s>
  + Returns a section of a string from a start and an optional end index.
  + Almost identical to `String.prototype.slice()`, use it instead.
+ ✅ `String.prototype.toLowerCase()`
+ ✅ `String.prototype.toUpperCase()`
+ ✅ `String.prototype.valueOf()`
  + Returns the primitive value of a String object.

#### ES3
+ ✅ `String.prototype.concat()`
+ ✅ `String.prototype.localeCompare()`
+ ✅ `String.prototype.match()`
+ ✅ `String.prototype.replace()`
+ ✅ `String.prototype.search()`
+ ✅ `String.prototype.slice()`
+ ✅ `String.prototype.split()`
  + Returns a section of a string from a start and an optional end index.
+ ✅ `String.prototype.substr()`
+ ✅ `String.prototype.toLocaleLowerCase()`
+ ✅ `String.prototype.toLocaleUpperCase()`
+ ✅ `String.prototype.toString()`

#### ES5.1
+ ✅ `String.prototype.trim()`
  + Removes whitespace from both ends of a string.

#### ES6
+ 🚧 `String.prototype.fromCodePoint()`
  + Returns a string from a sequence of code points.
+ ✅ `String.prototype.anchor()` <sup>HTML Wrapper</sup>
+ ❌ `String.prototype.big()` <sup>HTML Wrapper</sup>
+ ❌ `String.prototype.blink()` <sup>HTML Wrapper</sup>
+ ❌ `String.prototype.bold()` <sup>HTML Wrapper</sup>
+ 🚧 `String.prototype.codePointAt()`
+ 🚧 `String.prototype.endsWidth()`
+ ❌ `String.prototype.fixed()` <sup>HTML Wrapper</sup>
+ ❌ `String.prototype.fontcolor()` <sup>HTML Wrapper</sup>
+ ❌ `String.prototype.fontsize()` <sup>HTML Wrapper</sup>
+ 🚧 `String.prototype.includes()`
+ ❌ `String.prototype.italics()` <sup>HTML Wrapper</sup>
+ ✅ `String.prototype.link()` <sup>HTML Wrapper</sup>
+ 🚧 `String.prototype.normalize()`
+ 🚧 `String.prototype.repeat()`
+ ❌ `String.prototype.small()` <sup>HTML Wrapper</sup>
+ 🚧 `String.prototype.startsWith()`
+ ❌ `String.prototype.strike()` <sup>HTML Wrapper</sup>
+ ❌ `String.prototype.stub()` <sup>HTML Wrapper</sup>
+ ❌ `String.prototype.sup()` <sup>HTML Wrapper</sup>
+ 🚧 `String.prototype.[@@iterator]()`
+ 🚧 `String.prototype.raw()`

#### Non-standard
+ ❓ `String.prototype.quote()`
+ ❓ `String.prototype.toSource()`
+ ❓ `String.prototype.trimLeft()`
+ ❓ `String.prototype.trimRight()`

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
