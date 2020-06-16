# Debuggercises 

## /exercises/02-primitive-types/exercises 

> 6/16/2020, 2:21:44 PM 

[../README.md](../README.md)

- [/fill-in-the-type.js](#fill-in-the-typejs)  

---

## /fill-in-the-type.js 

>  
>
> [review source](../../../exercises/02-primitive-types/exercises/fill-in-the-type.js)

```txt
LOG: -- example --
LOG: object  null
LOG: object  null
LOG: -- challenge1 --
LOG: string  undefined
LOG: string  undefined
LOG: -- challenge2 --
LOG: number  Infinity
LOG: number  Infinity
LOG: -- challenge3 --
LOG: number  4
LOG: number  4
LOG: -- challenge4 --
LOG: string  4
LOG: string  4
LOG: -- challenge5 --
LOG: string  string
LOG: string  string
```

```js
'use strict';

// replace the _'s to complete the challenges
//  you know it's right when your log matches the one below it


console.log('-- example --');
const example = null;
console.log('object', null);
console.log(typeof example, example);

console.log('-- challenge1 --');
const challenge1 = 'undefined';
console.log('string','undefined');
console.log(typeof challenge1, challenge1);

console.log('-- challenge2 --');
const challenge2 = Infinity;
console.log('number', Infinity);
console.log(typeof challenge2, challenge2);

console.log('-- challenge3 --');
const challenge3 = 4;
console.log('number', 4);
console.log(typeof challenge3, challenge3);

console.log('-- challenge4 --');
const challenge4 = '4';
console.log('string','4');
console.log(typeof challenge4, challenge4);

console.log('-- challenge5 --');
const challenge5 = (typeof (typeof false));
console.log("string", 'string');
console.log(typeof challenge5, challenge5);


```

[TOP](#debuggercises)

