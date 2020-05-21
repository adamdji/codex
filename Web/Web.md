<!-- omit in toc -->
# Web

> Complex web technologies that overlap into different categories but must be together

<!-- omit in toc -->
## Index

- [Web Components](#web-components)
- [Web Assembly](#web-assembly)
- [Service Workers](#service-workers)
  - [What can it do](#what-can-it-do)
  - [Requirements](#requirements)
- [Web Workers](#web-workers)
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

---

## Web Assembly

---

## Service Workers

> 'Brains' behind an app to make it feel more native

### What can it do

- Create an offline experience
- Attach middleware to network connections
- Cache files
- Detect bad network connections are respond
- Convert file formats
- Replace the server if needed

### Requirements

- Compatible client browser
- Must be under a secured context (HTTPS at every point)
- One `js` file will be the worker
- Page in the scope to register the worker
- Will not work in private mode

---

## Web Workers

---

## APIs

### Drag and Drop

1. Set `draggable` attribute on an element to `true`; for any element
2. Set `ondragstart` attribute to a JS function, use the `event.dataTransfer` object in JS.
3. Set `ondragover` on an attribute that can have an item dragged over it to JS function, `preventDefault`
4. Set `ondrop` to event to handle the drop event.

> Call prevent default in each method (except `drag`)

## Accessibility
