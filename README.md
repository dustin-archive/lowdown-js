TLDR.js
=======
Unofficial opinionated TL;DR of JavaScript.

# Index
1. [Intro](#intro)
1. [Strings](#strings)
1. [Numbers](#numbers)
1. [Arrays](#arrays)
1. [Objects](#objects)
1. [Regex](#regex)
1. [Functions](#functions)
1. [Basic Conditionals](#basic-conditionals) (`if`, `else if`, etc)
1. [Loops](#Loops)
1. [Scoping](#scoping)
1. [Variables](#variables)
1. [Methods](#methods)
1. [Properties](#properties)

# Intro
Intro to JavaScript.

# Strings
## Single or double quotes?
Single quotes, meaning `'your string looks like this'`.

## `slice`, `substr`, and <s>`substring`</s>
+ `slice`
  + Use it if you know the start and end indexes.
  + Works on strings and arrays.
  + Allows a negative indexes.
+ `substr`
  + Use it if you know the start index and the length.
+ <s>`substring`</s>
  + Don't use it. It's just a dumb version of `slice`. Use `slice` instead.

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

# Functions

# Properties
## String
+ `.length`
  + Returns the length of a string.  

# Methods
## String
### ES1
+ `String.prototype.fromCharCode()`

### ES1
+ `String.prototype.charAt()`
+ `String.prototype.charCodeAt()`
+ `String.prototype.indexOf()`
+ `String.prototype.lastIndexOf()`
+ `String.prototype.substr()`
+ <s>`String.prototype.substring()`</s>
+ `String.prototype.toLocaleLowerCase()`
+ `String.prototype.toLocaleUpperCase()`
+ `String.prototype.toLowerCase()`
+ `String.prototype.toString()`
+ `String.prototype.toUpperCase()`
+ `String.prototype.trim()`
+ `String.prototype.valueOf()`
+ `String.prototype.raw()`

### ES3
+ `String.prototype.concat()`
+ `String.prototype.localeCompare()`
+ `String.prototype.match()`
+ `String.prototype.replace()`
+ `String.prototype.search()`
+ `String.prototype.slice()`
+ `String.prototype.split()`

### ES6
+ 💡`String.prototype.fromCodePoint()`
+ ✅`String.prototype.anchor()`
+ 💡`String.prototype.codePointAt()`
+ 💡`String.prototype.endsWidth()`
+ 💡`String.prototype.includes()`
+ ✅`String.prototype.link()`
+ 💡`String.prototype.normalize()`
+ 💡`String.prototype.repeat()`
+ 💡`String.prototype.startsWith()`
+ ❌`String.prototype.strike()`
+ 💡`String.prototype.[@@iterator]()`

### Deprecated
+ ❌`String.prototype.big()`
+ ❌`String.prototype.blink()`
+ ❌`String.prototype.bold()`
+ ❌`String.prototype.fixed()`
+ ❌`String.prototype.fontcolor()`
+ ❌`String.prototype.fontsize()`
+ ❌`String.prototype.italics()`
+ ❌`String.prototype.small()`
+ ❌`String.prototype.stub()`
+ ❌`String.prototype.sup()`

### Non-standard
+ ❓`String.prototype.quote()`
+ ❓`String.prototype.toSource()`
+ ❓`String.prototype.trimLeft()`
+ ❓`String.prototype.trimRight()`

# "Falsey" values
+ Don't use `undefined` in your code.
