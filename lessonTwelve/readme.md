# CSS learning

## 12. Lesson Twelve: Columns
Columns is a property that allows elements to be placed in columns. It is used to create layouts.

### 12.1. Columns
The columns property is used to create columns. It is used to create layouts.

```css
div {
  columns: 100px 3;
}
```
This will create 3 columns with a width of 100px.

### 12.2. Column Gap
The column-gap property is used to set the gap between the columns.

```css
div {
  column-gap: 40px;
}
```
This will set the gap between the columns to 40px.

### 12.3. Column Rule
The column-rule property is used to set the style of the rule between columns.

```css
div {
  column-rule: 2px solid red;
}
```
This will set the style of the rule between columns to 2px solid red. It is kinda like the border property.

### 12.4. Column Span
The column-span property is used to set the number of columns an element should span across.

```css
div {
  column-span: 2;
}
```
This will set the number of columns an element should span across to 2.

### 12.5. Column Fill
The column-fill property is used to set how the columns should be filled.

```css
div {
  column-fill: auto;
}
```
This will set how the columns should be filled to auto.

### 12.6. Column Width
The column-width property is used to set the width of the columns.

```css
div {
  column-width: 100px;
}
```
This will set the width of the columns to 100px.

### 12.7. Column Count
The column-count property is used to set the number of columns.

```css
div {
  column-count: 3;
}
```
This will set the number of columns to 3.

Note: columns is a shorthand property for `column-width` and `column-count`. 

### 12.8. Specificity
The columns property has a specificity of 1.
