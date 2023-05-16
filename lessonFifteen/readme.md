# CSS Learning

## Lesson Fifteen: Grid Layout

### 1. Grid Layout
Grid Layout in css is a very powerful tool for creating layouts. It is a 2-dimensional system, meaning it can handle both columns and rows, unlike flexbox which is largely a 1-dimensional system. You work with Grid Layout by applying CSS rules both to a parent element (which becomes the Grid Container) and to that elements children (which become Grid Items).
```css
.container {
  display: grid;
}
```
### 2. Grid Container
The element on which display: grid is applied. It’s the direct parent of all the grid items. In this example container is the grid container.
```css
.container {
  display: grid;
}
```
### 3. Grid Item
The children (i.e. direct descendants) of the grid container. Here the item elements are grid items, but sub-item isn’t.
```css
.item {
  display: grid;
}
```
### 4. Grid Line
The dividing lines that make up the structure of the grid. They can be either vertical (“column grid lines”) or horizontal (“row grid lines”) and reside on either side of a row or column. Here the yellow line is an example of a column grid line.
```css
.item {
  display: grid;
}
```
### 5. Grid Track
The space between two adjacent grid lines. You can think of them like the columns or rows of the grid. Here’s the grid track between the second and third row grid lines.
```css
.item {
  display: grid;
}
```
### 6. Grid Cell
The space between two adjacent row and two adjacent column grid lines. It’s a single “unit” of the grid. Here’s the grid cell between row grid lines 1 and 2, and column grid lines 2 and 3.
```css
.item {
  display: grid;
}
```
### 7. Grid Area
The total space surrounded by four grid lines. A grid area may be comprised of any number of grid cells. Here’s the grid area between row grid lines 1 and 3, and column grid lines 1 and 3.
```css
.item {
  display: grid;
}
```
### 8. Grid Properties
```css
.container {
  display: grid;
  grid-template-columns: 50px 50px 50px;
  grid-template-rows: 50px 50px;
}
```

### 9. Grid Template Columns
Defines the columns of the grid with a space-separated list of values. The values represent the track size, and the space between them represents the grid line. You can use absolute and relative lengths, as well as percentages, to size the columns. Here’s a grid with three columns sized at 100px, 3 columns sized at 20% of the container, and 3 columns sized at 1fr each.
```css
.container {
  display: grid;
  grid-template-columns: 100px 100px 100px 20% 20% 20% 1fr 1fr 1fr;
}
```
### 10. Grid Template Rows
Defines the rows of the grid with a space-separated list of values. The values represent the track size, and the space between them represents the grid line. You can use absolute and relative lengths, as well as percentages, to size the rows. Here’s a grid with three rows sized at 100px, 3 rows sized at 20% of the container, and 3 rows sized at 1fr each.
```css
.container {
  display: grid;
  grid-template-rows: 100px 100px 100px 20% 20% 20% 1fr 1fr 1fr;
}
```
### 11. Grid Template
A shorthand for setting grid-template-rows and grid-template-columns in a single declaration. Here’s a grid with 3 columns sized at 100px, 3 columns sized at 20% of the container, and 3 columns sized at 1fr each, and 3 rows sized at 100px, 3 rows sized at 20% of the container, and 3 rows sized at 1fr each.
```css
.container {
  display: grid;
  grid-template: 100px 100px 100px 20% 20% 20% 1fr 1fr 1fr / 100px 100px 100px 20% 20% 20% 1fr 1fr 1fr;
}
```
### 12. Grid Column Gap
Defines the size of the gap between the columns of the grid. You can think of it like setting the width of the gutters between the columns. Here’s a grid with a column gap of 20px.
```css
.container {
  display: grid;
  grid-column-gap: 20px;
}
```
### 13. Grid Row Gap
Defines the size of the gap between the rows of the grid. You can think of it like setting the height of the gutters between the rows. Here’s a grid with a row gap of 20px.
```css
.container {
  display: grid;
  grid-row-gap: 20px;
}
```
### 14. Grid Gap
A shorthand for grid-row-gap and grid-column-gap in a single declaration. Here’s a grid with a row gap of 20px and a column gap of 10px.
```css
.container {
  display: grid;
  grid-gap: 20px 10px;
}
```
### 15. Grid Template Areas
Defines named grid areas, establishing the cells in the grid and assigning them names. In order to define a grid area, you need to give the grid items within the grid a name and then use the grid-template-areas property on the grid container to specify its layout using the names you gave. Here’s a grid with three columns and three rows, and each cell named.
```css
.container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr 1fr;
  grid-template-areas:
    "header header header"
    "main main sidebar"
    "footer footer footer";
}

.item-a {
  grid-area: header;
}

.item-b {
  grid-area: main;
}

.item-c {
  grid-area: sidebar;
}

```
### 16. Grid Area
Gives an item a name so that it can be referenced by a template created with the grid-template-areas property. Here’s a grid with three columns and three rows, and each cell named.
```css
.container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr 1fr;
  grid-template-areas:
    "header header header"
    "main main sidebar"
    "footer footer footer";
}

.item-a {
  grid-area: header;
}

.item-b {
  grid-area: main;
}

.item-c {
  grid-area: sidebar;
}
```
### 17. Justify Items
Aligns grid items along the inline (row) axis (as opposed to align-items which aligns along the block (column) axis). Here’s a grid where the items are justified to the right.
```css
.container {
  display: grid;
  justify-items: end;
}
```
### 18. Align Items
Aligns grid items along the block (column) axis (as opposed to justify-items which aligns along the inline (row) axis). Here’s a grid where the items are aligned to the bottom.
```css
.container {
  display: grid;
  align-items: end;
}
```
### 19. Place Items
A shorthand for align-items and justify-items in a single declaration. Here’s a grid where the items are aligned to the bottom and justified to the right.
```css
.container {
  display: grid;
  place-items: end;
}
```
### 20. Justify Content
Aligns the grid along the inline (row) axis. Here’s a grid where the content is justified to the right.
```css
.container {
  display: grid;
  justify-content: end;
}
```
### 21. Align Content
Aligns the grid along the block (column) axis. Here’s a grid where the content is aligned to the bottom.
```css
.container {
  display: grid;
  align-content: end;
}
```
### 22. Place Content
A shorthand for align-content and justify-content in a single declaration. Here’s a grid where the content is aligned to the bottom and justified to the right.
```css
.container {
  display: grid;
  place-content: end;
}
```
### 23. Grid Auto Columns
Specifies the size of any auto-generated grid columns. Here’s a grid where the auto-generated columns are 100px wide.
```css
.container {
  display: grid;
  grid-auto-columns: 100px;
}
```
### 24. Grid Auto Rows
Specifies the size of any auto-generated grid rows. Here’s a grid where the auto-generated rows are 100px tall.
```css
.container {
  display: grid;
  grid-auto-rows: 100px;
}
```
### 25. Grid Auto Flow
Specifies how auto-generated grid items are inserted into the grid. Here’s a grid where the auto-generated items are inserted by row.
```css
.container {
  display: grid;
  grid-auto-flow: row;
}
```
### 26. Grid
A shorthand for setting all of the following properties in a single declaration: grid-template-rows, grid-template-columns, grid-template-areas, grid-auto-rows, grid-auto-columns, and grid-auto-flow. Here’s a grid with three columns and three rows, and each cell named.
```css
.container {
  display: grid;
  grid: 1fr 1fr 1fr / 1fr 1fr 1fr;
}
```
### 27. Grid Column Start
Determines a grid item’s location within the grid by referring to specific grid lines. Here’s a grid where the item starts on the 2nd vertical grid line and ends on the 4th.
```css
.item {
  grid-column-start: 2;
  grid-column-end: 4;
}
```
### 28. Grid Column End
Determines a grid item’s location within the grid by referring to specific grid lines. Here’s a grid where the item starts on the 2nd vertical grid line and ends on the 4th.
```css
.item {
  grid-column-start: 2;
  grid-column-end: 4;
}
```
### 29. Grid Column
A shorthand for grid-column-start and grid-column-end in a single declaration. Here’s a grid where the item starts on the 2nd vertical grid line and ends on the 4th.
```css
.item {
  grid-column: 2 / 4;
}
```
### 30. Grid Row Start
Determines a grid item’s location within the grid by referring to specific grid lines. Here’s a grid where the item starts on the 2nd horizontal grid line and ends on the 4th.
```css
.item {
  grid-row-start: 2;
  grid-row-end: 4;
}
```
### 31. Grid Row End
Determines a grid item’s location within the grid by referring to specific grid lines. Here’s a grid where the item starts on the 2nd horizontal grid line and ends on the 4th.
```css
.item {
  grid-row-start: 2;
  grid-row-end: 4;
}
```
### 32. Grid Row
A shorthand for grid-row-start and grid-row-end in a single declaration. Here’s a grid where the item starts on the 2nd horizontal grid line and ends on the 4th.
```css
.item {
  grid-row: 2 / 4;
}
```
### 33. Grid Area
A shorthand for grid-row-start, grid-column-start, grid-row-end and grid-column-end in a single declaration. Here’s a grid where the item starts on the 2nd vertical grid line and ends on the 4th, and starts on the 2nd horizontal grid line and ends on the 4th.
```css
.item {
  grid-area: 2 / 2 / 4 / 4;
}
```

Note: This can be overwelling at first, so complete the following exercises to get a better understanding of how to use grid. Link of the exercises: https://cssgridgarden.com/