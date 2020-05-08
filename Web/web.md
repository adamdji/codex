<!-- omit in toc -->
# General Web

<!-- omit in toc -->
## Index

- [Web Components](#web-components)
- [APIs](#apis)
  - [Drag and Drop](#drag-and-drop)
- [Accessibility](#accessibility)

---

## Web Components

<!-- omit in toc -->
### Templates

> `<template>` tag declares template markup that is not rendered directly onto a webpage

<!-- omit in toc -->
### Custom Elements

<!-- omit in toc -->
### Shadow DOM

## APIs

### Drag and Drop

1. Set `draggable` attribute on an element to `true`; for any element
2. Set `ondragstart` attribute to a JS function, use the `event.dataTransfer` object in JS.
3. Set `ondragover` on an attribute that can have an item dragged over it to JS function, `preventDefault`
4. Set `ondrop` to event to handle the drop event.

> Call prevent default in each method (except `drag`)

## Accessibility