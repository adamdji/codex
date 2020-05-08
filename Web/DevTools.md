<!-- omit in toc -->
# [Firefox](https://www.mozilla.org/en-US/firefox/developer/) DevTools [(Chrome)](https://developers.google.com/web/tools/chrome-devtools)

<!-- omit in toc -->
## Index

- [Page Inspector](#page-inspector)
- [Console](#console)
- [Debugger](#debugger)
- [Network Monitor](#network-monitor)
- [Storage Panel](#storage-panel)
- [Responsive Design Mode](#responsive-design-mode)
- [Visual Editing](#visual-editing)
- [Performance](#performance)
- [Memory](#memory)
- [Style Editor](#style-editor)
  - [Grid Inspector](#grid-inspector)
- [Accessibility](#accessibility)

---

## [Page Inspector](https://developer.mozilla.org/en-US/docs/Tools/Page_Inspector)

- Font inspector can edit fonts as it's on the webpage
- In `changes` tab, can see all custom changes made to copy into CSS file
- `Ctrl + Shift + C` toggles selector on or off
- [Various Keyboard shortcuts](https://developer.mozilla.org/en-US/docs/Tools/Page_Inspector/Keyboard_shortcuts#Breadcrumbs_bar)
- Breadcrumbs at the bottom, hover over to see which element
- Search elements using CSS Selectors or XPaths
- Inspect `::before` and `::after`
- View custom element definitions in debugger
- Copy unique CSS Selector or full path to an element *(good for ad-hoc changes)*
- Copy menu on an element has quite a bit of options
- _**Useful:**_ Show dom properties, outputs the HTMLElement into the console!
- Use in console lets you interact with the node in real time JavaScript
- Paste has various options (inner HTML, outerHTML, before, after)
- Change pseudo class to trigger hover, visited, etc.
- Can edit values directly in the box model

---

## [Console](https://developer.mozilla.org/docs/Tools/Web_Console)

- use `$0` to get the currently selected element

---

## [Debugger](https://developer.mozilla.org/docs/Tools/Debugger)

- Search for file name with `Ctrl + P` can also look for function definitions with `@`
- Pretty Print minified code with `{ }` icon.
- Can set URL breakpoints for requests.
- XHR Breakpoints and log points (replace console.log), event breakpoints, DOM mutation
- Watch expressions on object properties

---

## [Network Monitor](https://developer.mozilla.org/docs/Tools/Network_Monitor)

- Edit and resend `HTTP` requests
- Filter requests to specific domains with `-`
- See difference of speed with cache vs no cache
- Import and Export HAR
- Block specific URLs
- Filter by content, URL, XHR, WebSockets
- Filter by properties using keyword and colon `status-code:404`
- Context menu on a request has multiple features (copy as fetch, resend, save as HAR, fetch in console)

---

## [Storage Panel](https://developer.mozilla.org/docs/Tools/Storage_Inspector)

---

## [Responsive Design Mode](https://developer.mozilla.org/docs/Tools/Responsive_Design_View)

---

## [Visual Editing](https://hacks.mozilla.org/2015/11/developer-edition-44-creative-tools-and-more)

---

## [Performance](https://developer.mozilla.org/docs/Tools/Performance)

---

## [Memory](https://developer.mozilla.org/docs/Tools/Memory)

---

## [Style Editor](https://developer.mozilla.org/docs/Tools/Style_Editor)

- If the color is a foreground color, the color picker tells you whether its contrast with the background color meets accessibility guidelines
- Click `F1` on compute property to open `MDN` definition
- Opening drop down will show which selector set the property and what style sheet it is in
- `SHIFT + Click` colored dot to change representation of color
- Can use arrow and page up/down to increase/decrease numeric rules while editing

### Grid Inspector

---

## [Accessibility](https://developer.mozilla.org/en-US/docs/Tools/Accessibility_inspector)
