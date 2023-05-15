# CSS Learning Course

## Lesson 1 

In this lesson we will learn about to use CSS with HTML.

### External Way
In this we create an external file then we link with HTML file.

```html
link rel="stylesheet" href="style.css"
```
This is the way to link CSS file with HTML file.

### Internal Way
In this we use style tag in HTML file.

```html
<style>
    h1{
        color: red;
    }
</style>
```
This is the way to use CSS in HTML file.

Important note:If we use internal and external both then the internal CSS will be given priority. So, we should use both of them together then which came later in HTML the browser will give priority to that.

### Inline Way
In this we use style attribute in HTML tag.

```html
<h1 style="color: red;">Hello World</h1>
```
This is the way to use CSS in HTML file.

important note:The highest priority is given to inline CSS. But we should not use inline CSS because it is not a good practice because we will like our HTML and CSS will be separated.


Note: We cannot get error in CSS file therefore, we use a site called [CSS Validator](https://jigsaw.w3.org/css-validator/).

