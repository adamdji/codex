<!-- omit in toc -->
# TypeScript

<!-- omit in toc -->
## Index

- [Types](#types)
  - [Basic Types](#basic-types)
  - [Interfaces](#interfaces)
  - [Utility Types](#utility-types)
  - [Advanced Types](#advanced-types)
- [General Type System](#general-type-system)
- [Functions](#functions)
- [Guards](#guards)

## Types

### Basic Types

- `primitives`
- `Array`
- `tuple`
- `any`: Describe type of variables that we do not know when we are writing. Essentially turns off the type checker.
- `never`: Values that never occur, such as return type of a function that always throws an error. Variables can also be `never` if type guards narrow them to having nothing.
- `unknown`
- `null/undefined`: With strict null checks, both are only assignble to `any` and their respective types.
- `object`: Represents any non-primitive type.
- `void`: Function return, if assigned to a variable only `null` (if strict null checks if not specified) or `undefined` may be assigned to the variable.

> Can assert a type like a cast `(someValue as string).length;`

<!-- omit in toc -->
#### Enums

> Organize a collection of related values. Compiles down into a mapping, or into constant strings depending on the `const` keyword.

- Enums can be number based (default) or string based
- `const` tells the compiler to replace calls to the Enum with their actual literal, can break some dynamic code. Use `--preserveConstEnums` to help prevent this while using `const`
- Can use `namespace` with `enum` to add static methods to an enum by naming both the same name and exporting f unctions

### Interfaces

- Index Signatures: Indicate that an interface can have other 'dynamic' properties
- Interfaces can be used for functions as well, for a class of functions.

### Utility Types

### Advanced Types

## General Type System

- `declare` that something does exist before you use it (jQuery `$`)
- `type` creates named types from other types: `type Size = [number, number];`
- `readonly` property for properties of objects
- Typescript turns nonsensical statements into compile time errors `[] + []`, `{} + []`, `"hello" - 1`
- Prevents comparisons of `strings` to `numbers`
- `== null` checks for both undefined and null
- Use `typeof x !== undefined` for global level variables
- Annoate types inline using `:{ /*Structure*/ }`

``` typescript
    const x: { y: string; z: number; };
    x = { y: 'y', z: 5};
```

- Structural Typing: An object is assignable to a type if it meets all of the requirements of the type, even if it has properties that are not in the type

## Functions

``` typescript
    let fst: (a: any, d: any) => any = (a, d) => a;
    let snd: <T, U>(a: T, d: U) => U = (a, d) => d.
```

## Guards

> Multiple way to assert that an object contains a property

- `instanceof` and `typeof` in an if block