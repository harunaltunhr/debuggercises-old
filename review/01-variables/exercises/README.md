# Debuggercises 

## /exercises/01-variables/exercises 

> 6/15/2020, 10:06:16 PM 

[../README.md](../README.md)

- [/1-let.js](#1-letjs)  
- [/2-let.js](#2-letjs)  
- [/3-let-or-const.js](#3-let-or-constjs)  
- [/4-let-or-const.js](#4-let-or-constjs)  
- [/5-let-or-const.js](#5-let-or-constjs)  

---

## /1-let.js 

>  
>
> [review source](../../../exercises/01-variables/exercises/1-let.js)

```txt
LOG: c
LOG: bc
LOG: bcd
LOG: abcd
LOG: abcde
```

```js
'use strict';

// practice using variables declared with let
//  fill in the blanks to log the commented values
// and don't just write the correct answer directly!
//  you should use firstFiveLetters to fill in one blank for each step

let firstFiveLetters="c";
console.log(firstFiveLetters); // should log "c"

firstFiveLetters = "b" + firstFiveLetters;
console.log(firstFiveLetters); // should log "bc"

firstFiveLetters = firstFiveLetters + "d";
console.log(firstFiveLetters); // should log "bcd"

firstFiveLetters = "a" + firstFiveLetters;
console.log(firstFiveLetters); // should log "abcd"

firstFiveLetters = firstFiveLetters + "e";
console.log(firstFiveLetters); // should log "abcde"

```

[TOP](#debuggercises)

---

## /2-let.js 

>  
>
> [review source](../../../exercises/01-variables/exercises/2-let.js)

```txt
LOG: chocolate cake
LOG: chocolate cake with frosting
LOG: chocolate cake with frosting and banana
```

```js
'use strict';

// practice using variables declared with let
//  fill in the blanks to log the commented values
// and don't just write the correct answer directly!
//  practice re-using values stored in variables to get the correct value

let fruit = 'banana';
let desert = 'cake';
let topping = 'frosting';

desert="chocolate "+desert;
console.log(desert); // should log 'chocolate cake'

desert=`${desert} with ${topping}` ;
console.log(desert); // should log 'chocolate cake with frosting'

desert=`${desert} and ${fruit}`;
console.log(desert); // should log 'chocolate cake with frosting and banana'

```

[TOP](#debuggercises)

---

## /3-let-or-const.js 

>  
>
> [review source](../../../exercises/01-variables/exercises/3-let-or-const.js)

```txt
LOG: undefined
LOG: birch
LOG: myrtle
LOG: aspen
LOG: blue
LOG: myrtle
LOG: oak
LOG: orange
```

```js
'use strict';

/* declare and assign variables as described in the comments

  pay close attention to how each variable is used!
  - is a variable assigned a value when it is declared?
  - is a variable reassigned later in the script?

  your challenge is to decide whether to use let or to use const
  - use let if
    the variable is declared without an assignment
    or the variable is ever reassigned later in the script
  - use const if
    the variable is declared with a value and never reassigned

*/

// declare a variable named aTree, don't assign a value!
let aTree;
console.log(aTree);

// assign the value "birch" to the variable aTree
aTree='birch';
console.log(aTree);

// declare a variable named turtle and assign it the name "myrtle"
const turtle='myrtle';
console.log(turtle);

// reassign aTree to "aspen"
aTree='aspen';
console.log(aTree)

// declare a variable named aColor with the value "blue"
let aColor='blue';
console.log(aColor);

// log the value of turtle
console.log(turtle);

// reassign aTree to "oak"
aTree='oak';
console.log(aTree);

// reassign aColor to "orange"
aColor='orange';
console.log(aColor);

```

[TOP](#debuggercises)

---

## /4-let-or-const.js 

>  
>
> [review source](../../../exercises/01-variables/exercises/4-let-or-const.js)

```txt
LOG: a
LOG: b
LOG: a
LOG: undefined
LOG: b
LOG: c
LOG: bd
LOG: a
```

```js
'use strict';

/* declare and assign variables as described in the comments

  pay close attention to how each variable is used!
  - is a variable assigned a value when it is declared?
  - is a variable reassigned later in the script?

  your challenge is to decide whether to use let or to use const
  - use let if
    the variable is declared without an assignment
    or the variable is ever reassigned later in the script
  - use const if
    the variable is declared with a value and never reassigned

*/


const x ='a';
console.log(x); // should print 'a'

let y ='b';
console.log(y); // should print 'b'

console.log(x); // should print 'a'

let z;
console.log(z); // should print undefined

console.log(y); // should print 'b'

z ='c';
console.log(z); // should print 'c'

y=y+'d';
console.log(y); // should print 'bd'

console.log(x); // should print 'a'

```

[TOP](#debuggercises)

---

## /5-let-or-const.js 

>  
>
> [review source](../../../exercises/01-variables/exercises/5-let-or-const.js)

```txt
LOG: chair
LOG: house
LOG: table
LOG: undefined
LOG: apple
LOG: house
LOG: table
LOG: apple, pear
```

```js
'use strict';

/* declare and assign variables as described in the comments

  pay close attention to how each variable is used!
  - is a variable assigned a value when it is declared?
  - is a variable reassigned later in the script?

  your challenge is to decide whether to use let or to use const
  - use let if
    the variable is declared without an assignment
    or the variable is ever reassigned later in the script
  - use const if
    the variable is declared with a value and never reassigned

*/

let furniture='chair';
console.log(furniture); // should log 'chair'

const building ='house';
console.log(building); // should log 'house'

furniture = 'table';
console.log(furniture); // should log 'table'

let food;
console.log(food); // should log undefined

food = 'apple';
console.log(food); // should log 'apple'

console.log(building); // should log 'house'

console.log(furniture); // should log 'table'

let fruits = `${food}, pear`  ;
console.log(fruits); // should log 'apple, pear'

```

[TOP](#debuggercises)

