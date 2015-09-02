TLDR.js
=======
Unofficial opinionated TL;DR of JavaScript.

# Index
1. [Intro](#intro)
1. [Strings](#strings)
1. [Loops](#Loops)

# Intro
Intro to JavaScript.

# Strings
## Single or Double quotes?
It doesn't matter... as long as you use single quotes.

## slice, substr, and substring
+ `slice`
  + Use it if you know the start and the end.
  + Works on strings and arrays.
  + Allows a negative index.
+ `substr`
  + Use it if you know the start and the length.
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

### Operational
+ `label`
  + Names the loop so you can hop to it with the `condition` statement.
+ `break`
  + Stops a loop.
+ `continue`
  + Moves to the next iteration.

## Arrays
+ `forEach`
  + Iterates through an array with `item, index` in the callback function.

# "Falsey" values
+ Don't use `undefined` in your code.
