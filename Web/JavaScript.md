<!-- omit in toc -->
# JavaScript

<!-- omit in toc -->
## Index

- [Core](#core)
  - [Types](#types)
  - [Prototypes](#prototypes)
- [ECMAScript](#ecmascript)
  - [ES6](#es6)
  - [ES2016-ES2018](#es2016-es2018)
  - [ES2019-ESNext](#es2019-esnext)
- [DOM](#dom)
- [Web API's](#web-apis)
  - [Web Workers](#web-workers)
- [jQuery](#jquery)
- [Security](#security)

---

## Core

### Types

1. `Symbol`: Unique identifier, mainly for object properties

### Prototypes

> When it comes to inheritance, JavaScript only has one construct: objects. Each object has a private property which holds a link to another object called its prototype.
> 

---

## ECMAScript

### ES6

### ES2016-ES2018

<!-- omit in toc -->
#### ES2016 (ES7)

1. `Array.prototype.includes()`
2. Exponentiation Operator `**`

<!-- omit in toc -->
#### ES2017 (ES8)

1. `String.prototype.padStart(num)` and `String.prototype.padEnd(num)`
2. `Object.values(obj)`: Get an array containing all the object's own property values
3. `Object.entries(obj)`: Get an array containing object's own properties as `[key, val]`
4. `Object.getOwnPropertyDescriptors(obj)`: Return property descriptors of an object
5. Trailing commas
6. [Async/Await](###async/await)
7. Shared Memory and Atomics: Shared memory array between Web Workers and their creator, atomics enforce read / write consistency as in other languages.

<!-- omit in toc -->
#### ES2018 (ES9)

1. Rest/Spread for objects
2. `for-await-of` to use an async iterable object as a loop

### ES2019-ESNext

<!-- omit in toc -->
#### ES2019 (ES10)

1. `String.prototype.trimStart()` and `String.prototype.trimEnd()`
2. Optional Catch Binding
3. `Symbol.description`
4. Stable `Array.sort()` (TimSort)

<!-- omit in toc -->
#### ES2020 (ES11)

1. **BigInt**: Incredibly large number, denoted by adding an `n` at the end of a number.
2. **Dynamic Imports**: import module inside code when needed.
3. **Nullish Coalescing**: Check if something is `null` or `undefined`, if it is do something else.
4. **Optional Chaining**: Check deeply nested object properties without exessive if checking, if it does not exist undefined will be returned by the statement. Works with `functions` and `arrays`.
5. **Promise.allSettled**: Takes in an array of promises and resolves when all settled, res or rej.
6. **globalThis**: Returns the appropriate global object for the environment
   - `window` for browsers
   - `global` for Node
   - `self` for web workers

## DOM

---

## Web API's

### Web Workers

> Creates a separate JavaScript thread separate from the context of the main thread (no DOM, no synchronous API's)

---

## jQuery

---

## Security

<!-- omit in toc -->
### Secure Context

> `window.isSecureContext` A secure context is a Window or Worker for which there is reasonable confidence that the content has been delivered securely
