# CSS Learning

## Lesson Twenty: Variables

### Variables
- CSS variables are entities defined by CSS authors that contain specific values to be reused throughout a document.
- They are set using custom property notation (e.g., `--main-color: black;`) and are accessed using the `var()` function (e.g., `color: var(--main-color);`).
- CSS variables are case-sensitive, and their names are strings that represent the property name they are attached to.
- CSS variables are different from preprocessor variables. Preprocessor variables are static and cannot be changed once they are declared, whereas CSS variables are dynamic and can be changed at any time using JavaScript.
- CSS variables are supported in all modern browsers.
```css
:root {
  --main-bg-color: brown;
  --main-txt-color: white;
}

p {
  background-color: var(--main-bg-color);
  color: var(--main-txt-color);
}

```

In this we have root as the selector and then we have the variables defined in the root. Then we have the p selector and we have the background color and the color set to the variables. This is how we use variables in CSS.

