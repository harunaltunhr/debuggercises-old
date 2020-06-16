# Debuggercises 

## /exercises/04-value-swaps/exercises 

> 6/15/2020, 10:06:16 PM 

[../README.md](../README.md)

- [/1-double-swap.js](#1-double-swapjs) - _pass_ 
- [/2-triple-swap.js](#2-triple-swapjs) - _pass_ 
- [/3-triple-swap.js](#3-triple-swapjs) - _pass_ 
- [/4-quadruple-swap.js](#4-quadruple-swapjs) - _pass_ 
- [/5-quadruple-swap.js](#5-quadruple-swapjs) - _pass_ 
- [/6-let-and-const.js](#6-let-and-constjs) - _pass_ 
- [/7-let-and-const.js](#7-let-and-constjs) - _pass_ 

---

## /1-double-swap.js 

> pass 
>
> [review source](../../../exercises/04-value-swaps/exercises/1-double-swap.js)

```txt
+ PASS: Test 1
+ PASS: Test 2
+ PASS: Test 3
```

```js
'use strict';

let a = 2;
let b = 1;
let temp = null;

// write some code!
a=b;
b=b+a;

// fill in the _ to pass the assertions

const isTrue1 = a === 1;
console.assert(isTrue1, 'Test 1');

const isTrue2 = b === 2;
console.assert(isTrue2, 'Test 2');

const isTrue3 = temp === null;
console.assert(isTrue3, 'Test 3');


```

[TOP](#debuggercises)

---

## /2-triple-swap.js 

> pass 
>
> [review source](../../../exercises/04-value-swaps/exercises/2-triple-swap.js)

```txt
+ PASS: Test 1
+ PASS: Test 2
+ PASS: Test 3
+ PASS: Test 4
```

```js
'use strict';

let a = 3;
let b = 1;
let c = 2;
let temp = null;

// write some code!
a=b;
b=c;
c=c+a;


// fill in the _ to pass the assertions

const isTrue1 = a === 1;
console.assert(isTrue1, 'Test 1');

const isTrue2 = b === 2;
console.assert(isTrue2, 'Test 2');

const isTrue3 = c === 3;
console.assert(isTrue3, 'Test 3');

const isTrue4 = temp === null;
console.assert(isTrue4, 'Test 4');


```

[TOP](#debuggercises)

---

## /3-triple-swap.js 

> pass 
>
> [review source](../../../exercises/04-value-swaps/exercises/3-triple-swap.js)

```txt
+ PASS: Test 1
+ PASS: Test 2
+ PASS: Test 3
+ PASS: Test 4
```

```js
'use strict';

let a = 2;
let b = 3;
let c = 1;
let temp = null;

// write some code!
temp=b;
b=a;
a=c;
c=temp;



// fill in the _ to pass the assertions

const isTrue1 = a === 1;
console.assert(isTrue1, 'Test 1');

const isTrue2 = b === 2;
console.assert(isTrue2, 'Test 2');

const isTrue3 = c === 3;
console.assert(isTrue3, 'Test 3');

const isTrue4 = temp === 3;
console.assert(isTrue4, 'Test 4');


```

[TOP](#debuggercises)

---

## /4-quadruple-swap.js 

> pass 
>
> [review source](../../../exercises/04-value-swaps/exercises/4-quadruple-swap.js)

```txt
+ PASS: Test 1
+ PASS: Test 2
+ PASS: Test 3
+ PASS: Test 4
+ PASS: Test 5
```

```js
'use strict';

let a = 3;
let b = 4;
let c = 1;
let d = 2;
let temp = null;

// write some code!
temp=a;
a=c;
c=temp;
temp=b;
b=d;
d=temp;



// fill in the _ to pass the final assertions

const isTrue1 = a === 1;
console.assert(isTrue1, 'Test 1');

const isTrue2 = b === 2;
console.assert(isTrue2, 'Test 2');

const isTrue3 = c === 3;
console.assert(isTrue3, 'Test 3');

const isTrue4 = d === 4;
console.assert(isTrue4, 'Test 4');

const isTrue5 = temp === 4;
console.assert(isTrue5, 'Test 5');


```

[TOP](#debuggercises)

---

## /5-quadruple-swap.js 

> pass 
>
> [review source](../../../exercises/04-value-swaps/exercises/5-quadruple-swap.js)

```txt
+ PASS: Test 1
+ PASS: Test 2
+ PASS: Test 3
+ PASS: Test 4
+ PASS: Test 5
```

```js
'use strict';

let a = 3;
let b = 1;
let c = 4;
let d = 2;
let temp = null;

// write some code
temp=b;
b=d;
d=c;
c=a;
a=temp;

// fill in the final _ to pass the assertions

const isTrue1 = a === 1;
console.assert(isTrue1, 'Test 1');

const isTrue2 = b === 2;
console.assert(isTrue2, 'Test 2');

const isTrue3 = c === 3;
console.assert(isTrue3, 'Test 3');

const isTrue4 = d === 4;
console.assert(isTrue4, 'Test 4');

const isTrue5 = temp === 1;
console.assert(isTrue5, 'Test 5');


```

[TOP](#debuggercises)

---

## /6-let-and-const.js 

> pass 
>
> [review source](../../../exercises/04-value-swaps/exercises/6-let-and-const.js)

```txt
+ PASS: Test 1
+ PASS: Test 2
+ PASS: Test 3
+ PASS: Test 4
```

```js
'use strict';

// write code to pass asserts a and b
// fill in the blanks for c and temp

// leave this code as it is
let a = 2;
let b = 1;
let temp = null;

temp = a;
const c = temp;

// write your code below here, and above the assertions
a=b;
b=c;



// replace the _ with a value to pass the assertions

const isTrue1 = a === 1;
console.assert(isTrue1, "Test 1");

const isTrue2 = b === 2;
console.assert(isTrue2, "Test 2");

const isTrue3 = c === 2;
console.assert(isTrue3, "Test 3");

const isTrue4 = temp === 2;
console.assert(isTrue4, "Test 4");


```

[TOP](#debuggercises)

---

## /7-let-and-const.js 

> pass 
>
> [review source](../../../exercises/04-value-swaps/exercises/7-let-and-const.js)

```txt
+ PASS: Test 1
+ PASS: Test 2
+ PASS: Test 3
+ PASS: Test 4
+ PASS: Test 5
```

```js
'use strict';

// write code to pass asserts a, b, c
// fill in the blanks for d and temp

// leave this code as it is
let a = 2;
let b = 3;
let c = 1;
let temp = null;

temp = a;
a = b;
const d = a;
// write your code below here
a=c;
b=temp;
c=d;




// fill in in the _'s to pass the final assertions

const isTrue1 = a === 1;
console.assert(isTrue1, 'Test 1');

const isTrue2 = b === 2;
console.assert(isTrue2, 'Test 2');

const isTrue3 = c === 3;
console.assert(isTrue3, 'Test 3');

const isTrue4 = d === 3;
console.assert(isTrue4, 'Test 4');

const isTrue5 = temp === 2;
console.assert(isTrue5, 'Test 5');


```

[TOP](#debuggercises)

