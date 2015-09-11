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
