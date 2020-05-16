<!-- omit in toc -->
# TypeScript

<!-- omit in toc -->
## Index

- [Types](#types)
  - [Basic Types](#basic-types)
  - [Utility Types](#utility-types)
  - [Advanced Types](#advanced-types)
- [General Type System](#general-type-system)
- [Functions](#functions)

## Types

### Basic Types

- `any`: Essentially turns off the type checker
- `unknown`
- `never`
- `null/undefined`
- `primitives`
- `Array`
- `Object`
- `void`

### Utility Types

### Advanced Types

<!-- omit in toc -->
#### Enums

> Organize a collection of related values. Compiles down into a mapping, or into constant strings depending on the `const` keyword.

- Enums can be number based (default) or string based
- `const` tells the compiler to replace calls to the Enum with their actual literal, can break some dynamic code. Use `--preserveConstEnums` to help prevent this while using `const`
- Can use `namespace` with `enum` to add static methods to an enum by naming both the same name and exporting f unctions

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
