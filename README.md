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
       | <sub> Description </sub>
:----: | ------------------------
<sub> ✅ </sub> | <sub> Safe to use </sub>
<sub> ❎ </sub> | <sub> Safe to use but not recommended </sub>
<sub> 🚧 </sub> | <sub> Some support </sub>
<sub> ❌ </sub> | <sub> Deprecated </sub>
<sub> ❓ </sub> | <sub> Non-standard </sub>

## String
### Properties
#### ES1
       | <sub> Name </sub> | <sub> Info </sub>
:----: | ----------------- | -----------------
<sub> ✅ </sub> | <sub> `String.length` </sub> | <sub> 🔹 Returns the length of a string. </sub>
<sub> ✅ </sub> | <sub> `String.prototype` </sub> | <sub> 🔹 Represents the string prototype object. </sub>

### Methods
#### ES1
       | <sub> Name </sub> | <sub> Info </sub>
:----: | ----------------- | -----------------
<sub> ❎ </sub> | <sub> ~~`String.prototype.fromCharCode()`~~ </sub> | <sub> 🔹 Returns a string from a sequence of Unicode values. <br> 🔹 Cannot return all Unicode characters. <br> 🔹 Use `String.fromCodePoint()` instead. </sub>
<sub> ✅ </sub> | <sub> `String.prototype.charAt()` </sub>
<sub> ✅ </sub> | <sub> `String.prototype.charCodeAt()` </sub>
<sub> ✅ </sub> | <sub> `String.prototype.indexOf()` </sub>
<sub> ✅ </sub> | <sub> `String.prototype.lastIndexOf()` </sub>
<sub> ❎ </sub> | <sub> ~~`String.prototype.substring()`~~ </sub> | <sub> 🔹 Returns a section of a string from a start and an optional end index. <br> 🔹 Almost identical to `String.prototype.slice()`, use it instead. </sub>
<sub> ✅ </sub> | <sub> `String.prototype.toLowerCase()` </sub>
<sub> ✅ </sub> | <sub> `String.prototype.toUpperCase()` </sub>
<sub> ✅ </sub> | <sub> `String.prototype.valueOf()` </sub> | <sub> 🔹 Returns the primitive value of a String object. </sub>

#### ES3
       | <sub> Name </sub> | <sub> Info </sub>
:----: | ----------------- | -----------------
<sub> ✅ </sub> | <sub> `String.prototype.concat()` </sub>
<sub> ✅ </sub> | <sub> `String.prototype.localeCompare()` </sub>
<sub> ✅ </sub> | <sub> `String.prototype.match()` </sub>
<sub> ✅ </sub> | <sub> `String.prototype.replace()` </sub>
<sub> ✅ </sub> | <sub> `String.prototype.search()` </sub>
<sub> ✅ </sub> | <sub> `String.prototype.slice()` </sub>
<sub> ✅ </sub> | <sub> `String.prototype.split()` </sub> | <sub> 🔹 Returns a section of a string from a start and an optional end index. </sub>
<sub> ✅ </sub> | <sub> `String.prototype.substr()` </sub>
<sub> ✅ </sub> | <sub> `String.prototype.toLocaleLowerCase()` </sub>
<sub> ✅ </sub> | <sub> `String.prototype.toLocaleUpperCase()` </sub>
<sub> ✅ </sub> | <sub> `String.prototype.toString()` </sub>

#### ES5.1
       | <sub> Name </sub> | <sub> Info </sub>
:----: | ----------------- | -----------------
<sub> ✅ </sub> | <sub> `String.prototype.trim()` </sub> | <sub> 🔹 Removes whitespace from both ends of a string. </sub>

#### ES6

##### Not HTML
       | <sub> Name </sub> | <sub> Info </sub>
:----: | ----------------- | -----------------
<sub> 🚧 </sub> | <sub> `String.prototype.fromCodePoint()` </sub> | <sub> 🔹 Returns a string from a sequence of code points. </sub>
<sub> 🚧 </sub> | <sub> `String.prototype.codePointAt()` </sub>
<sub> 🚧 </sub> | <sub> `String.prototype.endsWidth()` </sub>
<sub> 🚧 </sub> | <sub> `String.prototype.includes()` </sub>
<sub> 🚧 </sub> | <sub> `String.prototype.normalize()` </sub>
<sub> 🚧 </sub> | <sub> `String.prototype.repeat()` </sub>
<sub> 🚧 </sub> | <sub> `String.prototype.startsWith()` </sub>
<sub> 🚧 </sub> | <sub> `String.prototype.[@@iterator]()` </sub>
<sub> 🚧 </sub> | <sub> `String.prototype.raw()` </sub>

##### HTML Wrappers
       | <sub> Name </sub> | <sub> Info </sub>
:----: | ----------------- | -----------------
<sub> ✅ </sub> | <sub> `String.prototype.anchor()` </sub>
<sub> ❌ </sub> | <sub> ~~`String.prototype.big()`~~ </sub>
<sub> ❌ </sub> | <sub> ~~`String.prototype.blink()`~~ </sub>
<sub> ❌ </sub> | <sub> ~~`String.prototype.bold()`~~ </sub>
<sub> ❌ </sub> | <sub> ~~`String.prototype.fixed()`~~ </sub>
<sub> ❌ </sub> | <sub> ~~`String.prototype.fontcolor()`~~ </sub>
<sub> ❌ </sub> | <sub> ~~`String.prototype.fontsize()`~~ </sub>
<sub> ❌ </sub> | <sub> ~~`String.prototype.italics()`~~ </sub>
<sub> ✅ </sub> | <sub> `String.prototype.link()` </sub>
<sub> ❌ </sub> | <sub> ~~`String.prototype.small()`~~ </sub>
<sub> ❌ </sub> | <sub> ~~`String.prototype.strike()`~~ </sub>
<sub> ❌ </sub> | <sub> ~~`String.prototype.stub()`~~ </sub>
<sub> ❌ </sub> | <sub> ~~`String.prototype.sup()`~~ </sub>

#### Non-standard
       | <sub> Name </sub> | <sub> Info </sub>
:----: | ----------------- | -----------------
<sub> ❓ </sub> | <sub> ~~`String.prototype.quote()`~~ </sub>
<sub> ❓ </sub> | <sub> ~~`String.prototype.toSource()`~~ </sub>
<sub> ❓ </sub> | <sub> ~~`String.prototype.trimLeft()`~~ </sub>
<sub> ❓ </sub> | <sub> ~~`String.prototype.trimRight()`~~ </sub>

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
