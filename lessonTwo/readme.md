# CSS Learning

## 2. Lesson Two
In this Lesson we are going to use learn about CSS Selectors.

### Least Specific to Most Specific

1. Universal Selector
   ```css
    * {
      color: red;
    }
    ```
In this example, the `*` is the universal selector. It will select all elements on the page.

Note: It is not inheritaded the value, it is just selecting all the values.

It is not recommended to use the universal selector. But, it can use only to reset the CSS design.


2. Type Selector
    ```css
    p {
      color: red;
    }

    div {
      color: green;
    }

    h1 {
      color: blue;
    }

    body {
      color: yellow;
    }
    ```
In this example, the `p`, `div`, `h1` and `body` are the type selectors. It will select all the elements with the same type. It has a higher specificity than the universal selector but lower than the class and id selectors.

Some Values can be inherited like color, font-size, font-family, etc. But, some values can not be inherited like border, margin, padding, etc. 

Note: If you wanted to make some value not inherited to inherit, you can use the `inherit` value.

3. Class Selector
    ```html
    <!-- Inside index.html -->
    <p class="red">This is a paragraph</p>
    <p class="green">This is a paragraph</p>
    <p class="blue">This is a paragraph</p>
    <p class="yellow">This is a paragraph</p>
    ```
    ```css
    <!-- Inside style.css -->
    .red {
      color: red;
    }

    .green {
      color: green;
    }

    .blue {
      color: blue;
    }

    .yellow {
      color: yellow;
    }
    ```

In this example, the `.red`, `.green`, `.blue` and `.yellow` are the class selectors. It will select all the elements with the same class. It has a higher specificity than the type selector but lower than the id selector.

4. ID Selector
    ```html
    <!-- Inside index.html -->
    <p id="red">This is a paragraph</p>
    <p id="green">This is a paragraph</p>
    <p id="blue">This is a paragraph</p>
    <p id="yellow">This is a paragraph</p>
    ```
    ```css
    <!-- Inside style.css -->
    #red {
      color: red;
    }

    #green {
      color: green;
    }

    #blue {
      color: blue;
    }

    #yellow {
      color: yellow;
    }
    ```
In this example, the `#red`, `#green`, `#blue` and `#yellow` are the id selectors. It will select all the elements with the same id. It has a higher specificity than the class selector but lower than the inline style.

Note: It is not recommended to use the id selector. 
Reason: It can voilate the DRY principle. It can be used only for the JavaScript.
