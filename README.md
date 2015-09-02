TLDR.js
=======
Unofficial opinionated TL;DR of JavaScript.

# Index
1. [Intro](#intro)
1. [Strings](#strings)
1. [Loops](#Loops)
1. [Functions](#functions)

# Intro
Intro to JavaScript.

# Strings
## Single or Double quotes?
It doesn't matter... as long as you use single quotes.

## slice, substr, and substring
+ `slice` Use it if you know the start and the end.
+ `substr` Use it if you know the start and the length.
+ `substring` Don't use it because it's just a dumb version of `slice`.

# Loops
## Statements
### Conditional
#### `for`
+ Use it when you know the start and end of a loop.

+ `for...in`
  + Enumerate over an object.
  + Discouraged for arrays. Use `for...of` instead.
+ `for...of`
  + Enumerate arrays and objects.
+ <s>`for each...in`</s>
  + Don't use it because it's obsolete. Use `for...of` instead.

#### `while`
Use it when you know the start but not the end of a loop.

+ `do...while`
  + Execute block once before loop.
  + Use it when you want to to manipulate the iterator in the loop itself.

### Operational
+ `label`
  + Name the loop so you can hop to it with the `condition` statement.
+ `break`
  + Stop a loop.
+ `continue`
  + Move to the next iteration.

## Arrays
+ `forEach`
  + Iterates through an array with `item, index` in the callback function.

# Functions

# "Falsey" values
+ Don't use 'undefined' in your code.
