# CSS Learning  
## Lesson 19: Pesudo-classes and Pesudo-elements

### Pesudo-classes
- A pseudo-class is used to define a special state of an element.
- For example, it can be used to:
  - Style an element when a user mouses over it
  - Style visited and unvisited links differently
  - Style an element when it gets focus
- Syntax: `selector:pseudo-class {property:value;}`
- Example: `a:hover {color: red;}`
- Example: `a:visited {color: green;}`
- Example: `a:focus {color: blue;}`
- Example: `input:required {background: yellow;}`
- Example: `input:optional {background: yellow;}`
- Example: `input:checked {background: yellow;}`
- Example: `input:disabled {background: yellow;}`
- Example: `input:enabled {background: yellow;}`


### Pesudo-elements
- A pseudo-element is used to style specified parts of an element.

- For example, it can be used to:
  - Style the first letter, or line, of an element
  - Insert content before, or after, the content of an element
  - Syntax: `selector::pseudo-element {property:value;}`
    - Example: `p::first-line {color: blue;}`
    - Example: `p::first-letter {color: blue;}`
    - Example: `p::before {content: url(smiley.gif);}`
    - Example: `p::after {content: url(smiley.gif);}`
    - Example: `p::before {content: "Read this: ";}`
    - Example: `p::after {content: " - end of section";}`
    - Example: `p::first-letter {font-size: xx-large;}`
    - Example: `p::first-line {font-variant: small-caps;}`
    - Example: `p::first-letter {font-style: italic;}`
    - Example: `p::first-letter {font-weight: bold;}`
    - Example: `p::first-letter {color: #ff0000;}`
    - Example: `p::first-letter {background-color: #ff0000;}`
    - Example: `p::first-letter {text-transform: uppercase;}`
    - Example: `p::first-letter {padding: 10px;}`
