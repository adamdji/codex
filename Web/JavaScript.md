<!-- omit in toc -->
# JavaScript

<!-- omit in toc -->
## Index

- [Core](#core)
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

---

## ECMAScript

### ES6

### ES2016-ES2018

### ES2019-ESNext

<!-- omit in toc -->
#### ES2019

**`String.trimStart()` and `String.trimEnd()`**

**Optional Catch Binding**

**`Symbol.description`**

**Stable `Array.sort()` (TimSort)**

<!-- omit in toc -->
#### ES2020

**BigInt**: Incredibly large number, denoted by adding an `n` at the end of a number.
  
```javascript
let newNum = 9007199254740992n;
```

**Dynamic Imports**: import module inside code when needed.

```javascript
const module = await import('./myModule.js');
```

**Nullish Coalescing**: Check if something is `null` or `undefined`, if it is do something else.

```javascript
undefined ?? doSomethingElse();
```

**Optional Chaining**: Check deeply nested object properties without exessive if checking, if it does not exist undefined will be returned by the statement. Works with `functions` and `arrays`.

```javascript
const x = {y: { z: [2, 3] } }
x?.y?.z[1];
```

**Promise.allSettled**: Takes in an array of promises and resolves when all settled, res or rej.

**globalThis**: Returns the appropriate global object for the environment

1. `window` for browsers
2. `global` for Node
3. `self` for web workers

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
