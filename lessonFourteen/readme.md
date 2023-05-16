# CSS learning

## 14. Lesson Fourteen: Flexbox

### 14.1. What is Flexbox?
Flexbox is a layout mode of CSS3. It is designed for laying out more complex applications and web pages. It is used for positioning and aligning items within a container. It is a one-dimensional layout method for laying out items in rows or columns. Items flex to fill additional space and shrink to fit into smaller spaces. Flexbox is a whole module and not a single property. In the past, layout was accomplished using **floats** and **positioning**. Flexbox is a new layout mode in CSS3. It is a set of properties, applied to a parent element, that controls the layout and sizing of its children. The flexible box layout module makes it easier to design flexible responsive layout structure without using float or positioning.

### 14.2. Flexbox Properties
Flexbox is a whole module and not a single property. To start using Flexbox, you need to first define a flex container. The flex container becomes flexible by setting the display property to flex. The flex container properties are as follows:

- **display**: This defines a flex container. It enables a flex context for all its direct children. It also enables display: block. It is a block-level element.
    ```css
    .container {
        display: flex;
    }
    ```

- **flex-direction**: This establishes the main-axis, thus defining the direction flex items are placed in the flex container. It is similar to the direction property of the flex container. It is a container property.
    ```css
    .container {
        flex-direction: row | row-reverse | column | column-reverse;
    }
    ```
- **flex-wrap**: This controls whether flex items are forced into a single line or can be wrapped into multiple lines. It is a container property.
    ```css
    .container {
        flex-wrap: nowrap | wrap | wrap-reverse;
    }
    ```
- **flex-flow**: This is a shorthand for the flex-direction and flex-wrap properties. It is a container property.
    ```css
    .container {
        flex-flow: <flex-direction> || <flex-wrap>;
    }
    ```

- **justify-content**: This defines the alignment along the main-axis. It helps distribute extra free space left over when either all the flex items on a line are inflexible, or are flexible but have reached their maximum size. It is a container property.
    ```css
    .container {
        justify-content: flex-start | flex-end | center | space-between | space-around;
    }
    ```
- **align-items**: This defines the default behavior for how flex items are laid out along the cross axis on the current line. It is a container property.
    ```css
    .container {
        align-items: flex-start | flex-end | center | baseline | stretch;
    }
    ```
- **align-content**: This aligns a flex container's lines within when there is extra space in the cross-axis, similar to how justify-content aligns individual items within the main-axis. It is a container property.
    ```css
    .container {
        align-content: flex-start | flex-end | center | space-between | space-around | stretch;
    }
    ```


Now you have to completed a game of flexbox froggy. You can play it [here](https://flexboxfroggy.com/).