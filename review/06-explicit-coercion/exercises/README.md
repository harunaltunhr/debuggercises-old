# Debuggercises 

## /exercises/06-explicit-coercion/exercises 

> 6/16/2020, 2:21:44 PM 

[../README.md](../README.md)

- [/1-write-expected.js](#1-write-expectedjs) - _pass_ 
- [/2-write-arguments.js](#2-write-argumentsjs) - _pass_ 
- [/3-write-function.js](#3-write-functionjs) - _pass_ 

---

## /1-write-expected.js 

> pass 
>
> [review source](../../../exercises/06-explicit-coercion/exercises/1-write-expected.js)

```txt
+ PASS: Test 1
+ PASS: Test 2
+ PASS: Test 3
+ PASS: Test 4
+ PASS: Test 5
+ PASS: Test 6
+ PASS: Test 7
+ PASS: Test 8
+ PASS: Test 9
```

```js
'use strict';

function mystery(x) {
  if (typeof x === 'boolean') { throw new TypeError('x cannot be a boolean'); }

  const booleaned = Boolean(x);
  const numbered = Number(booleaned);
  return numbered;
}

// write the expected return value

const _1_expect = 0;
const _1_actual = mystery(undefined);
console.assert(_1_actual === _1_expect, 'Test 1');

const _2_expect = 0;
const _2_actual = mystery(null);
console.assert(_2_actual === _2_expect, 'Test 2');

const _3_expect = 1;
const _3_actual = mystery('false');
console.assert(_3_actual === _3_expect, 'Test 3');

const _4_expect = 0;
const _4_actual = mystery('');
console.assert(_4_actual === _4_expect, 'Test 4');

const _5_expect = 0;
const _5_actual = mystery(0);
console.assert(_5_actual === _5_expect, 'Test 5');

const _6_expect = 1;
const _6_actual = mystery('  ');
console.assert(_6_actual === _6_expect, 'Test 6');

const _7_expect = 1;
const _7_actual = mystery(-1);
console.assert(_7_actual === _7_expect, 'Test 7');

const _8_expect = 1;
const _8_actual = mystery('true');
console.assert(_8_actual === _8_expect, 'Test 8');

const _9_expect = 1;
const _9_actual = mystery(1);
console.assert(_9_actual === _9_expect, 'Test 9');


```

[TOP](#debuggercises)

---

## /2-write-arguments.js 

> pass 
>
> [review source](../../../exercises/06-explicit-coercion/exercises/2-write-arguments.js)

```txt
+ PASS: Test 1
+ PASS: Test 2
+ PASS: Test 3
+ PASS: Test 4
+ PASS: Test 5
+ PASS: Test 6
+ PASS: Test 7
+ PASS: Test 8
+ PASS: Test 9
```

```js
'use strict';

function mystery(x) {
  if (typeof x === 'string') { throw new TypeError('x cannot be a string'); }

  const stringed = String(x);
  const numbered = Number(stringed);
  return numbered;
}

// find an argument to get the expected return value

const _1_expect = -1;
const _1_actual = mystery(-1);
console.assert(Object.is(_1_actual, _1_expect), 'Test 1');

const _2_expect = 0;
const _2_actual = mystery(0);
console.assert(Object.is(_2_actual, _2_expect), 'Test 2');

const _3_expect = 1;
const _3_actual = mystery(1);
console.assert(Object.is(_3_actual, _3_expect), 'Test 3');

const _4_expect = 0.5;
const _4_actual = mystery(0.5);
console.assert(Object.is(_4_actual, _4_expect), 'Test 4');

const _5_expect = 1000;
const _5_actual = mystery(1000);
console.assert(Object.is(_5_actual, _5_expect), 'Test 5');

const _6_expect = NaN;
const _6_actual = mystery(NaN);
console.assert(Object.is(_6_actual, _6_expect), 'Test 6');

const _7_expect = NaN;
const _7_actual = mystery(NaN);
console.assert(Object.is(_7_actual, _7_expect), 'Test 7');

const _8_expect = NaN;
const _8_actual = mystery(undefined);
console.assert(Object.is(_8_actual, _8_expect), 'Test 8');

const _9_expect = NaN;
const _9_actual = mystery(null);
console.assert(Object.is(_9_actual, _9_expect), 'Test 9');


```

[TOP](#debuggercises)

---

## /3-write-function.js 

> pass 
>
> [review source](../../../exercises/06-explicit-coercion/exercises/3-write-function.js)

```txt
+ PASS: Test 1
+ PASS: Test 2
+ PASS: Test 3
+ PASS: Test 4
+ PASS: Test 5
+ PASS: Test 6
+ PASS: Test 7
+ PASS: Test 8
+ PASS: Test 9
```

```js
'use strict';

/* write a function to pass the test cases
  it can be solved using only
   Number
   ===
*/
function mystery(x, y) {
 return Number(x)===Number(y);
}


// all of the test cases are correct

const _1_expect = true;
const _1_actual = mystery('', '');
console.assert(_1_actual === _1_expect, 'Test 1');

const _2_expect = true;
const _2_actual = mystery(false, null);
console.assert(_2_actual === _2_expect, 'Test 2');

const _3_expect = false;
const _3_actual = mystery('asdf', 'asdf');
console.assert(_3_actual === _3_expect, 'Test 3');

const _4_expect = true;
const _4_actual = mystery('1.0', '1');
console.assert(_4_actual === _4_expect, 'Test 4');

const _5_expect = false;
const _5_actual = mystery(false, true);
console.assert(_5_actual === _5_expect, 'Test 5');

const _6_expect = false;
const _6_actual = mystery('1.5', '1');
console.assert(_6_actual === _6_expect, 'Test 6');

const _7_expect = true;
const _7_actual = mystery('1e3', '1000');
console.assert(_7_actual === _7_expect, 'Test 7');

const _8_expect = true;
const _8_actual = mystery(false, '');
console.assert(_8_actual === _8_expect, 'Test 8');

const _9_expect = false;
const _9_actual = mystery(undefined, undefined);
console.assert(_9_actual === _9_expect, 'Test 9');


```

[TOP](#debuggercises)

