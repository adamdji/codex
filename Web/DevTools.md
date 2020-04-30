# FireFox DevTools

## [Page Inspector](https://developer.mozilla.org/en-US/docs/Tools/Page_Inspector)

- Font inspector can edit fonts as it's on the webpage
- In `changes` tab, can see all custom changes made to copy into CSS file
- `Ctrl + Shift + C` toggles selector on or off
- Various Keyboard shortcuts [here](https://developer.mozilla.org/en-US/docs/Tools/Page_Inspector/Keyboard_shortcuts#Breadcrumbs_bar)
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

### Styling

- If the color is a foreground color, the color picker tells you whether its contrast with the background color meets accessibility guidelines
- Click `F1` on compute property to open `MDN` definition
- Opening drop down will show which selector set the property and what style sheet it is in
- `SHIFT + Click` colored dot to change representation of color
- Can use arrow and page up/down to increase/decrease numeric rules while editing

## Console

- use `$0` to get the currently selected element

## Debugger

- Search for file name with `Ctrl + P` can also look for function definitions with `@`
- Pretty Print minified code with `{ }` icon.
- Can set URL breakpoints for requests.

## Network Monitor

- Edit and resend `HTTP` requests
- Filter requests to specific domains with `-`
- See difference of speed with cache vs no cache
- Import and Export HAR
