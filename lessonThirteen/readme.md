# CSS Learning

## 13. Lesson Thirteen: Position

### 13.1. Position
Postion is a property that allows you to control the location of an element in the page. It has 5 values:
- static
    ```css
    position: static;
    ```
This is the default value. It means that the element will be placed in the page according to the normal flow of the document. It will not be affected by the top, bottom, left, right properties.


- relative
    ```css
    position: relative;
    ```
This value allows you to move the element from its normal position. It will be moved according to the top, bottom, left, right properties. It will not affect the position of other elements.

- absolute
    ```css
    position: absolute;
    ```
This value allows you to move the element from its normal position. It will be moved according to the top, bottom, left, right properties. It will affect the position of other elements.

- fixed
    ```css
    position: fixed;
    ```
This value allows you to move the element from its normal position. It will be moved according to the top, bottom, left, right properties. It will affect the position of other elements. The difference between absolute and fixed is that fixed is relative to the viewport, while absolute is relative to the parent element.

- sticky
    ```css
    position: sticky;
    ```
This value allows you to move the element from its normal position. It will be moved according to the top, bottom, left, right properties. It will affect the position of other elements. The difference between sticky and fixed is that sticky is relative to the parent element, while fixed is relative to the viewport.
