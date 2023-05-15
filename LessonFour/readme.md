# CSS learning

## 4. Lesson Four: Unit and Size

There are many units and size in css to define the size of elements. The most common units are px, em, rem, %, vw, vh, vmin, vmax.

### 4.1 px
px is the most common unit in css. It is a fixed size. 1px is 1/96 inch. It is not recommended to use px to define the size of elements. Because it is not responsive. It is not good for different screen size.

```css

div {
    width: 100px;
    height: 100px;
}

```


### 4.2 em

em is a relative unit. It is relative to the font size of the parent element. If the font size of the parent element is 16px, 1em is 16px. If the font size of the parent element is 20px, 1em is 20px.

```css
div {
    font-size: 16rm;
    /* It will take parent size let assume it is 16px then it will mulitiply by 16
    
        1em = 16px
        16em = 216px
    */
}
```

### 4.3 rem
rem is a relative unit. It is relative to the font size of the root element. The root element is the html element. The default font size of the html element is 16px. If the font size of the html element is 16px, 1rem is 16px. If the font size of the html element is 20px, 1rem is 20px.

```css
div {
    font-size: 16rem;
    /* It will take root size let assume it is 16px then it will mulitiply by 16 by default in browser
    
        1rem = 16px
        16rem = 216px
    */
}
```


### 4.4 %

% is a relative unit. It is relative to the size of the parent element. If the size of the parent element is 100px, 50% is 50px. If the size of the parent element is 200px, 50% is 100px.

```css
div {
    width: 50%;
    /* It will take parent size let assume it is 100px then it will mulitiply by 50
    
        50% = 50px
    */
}
```


### 4.5 vw

vm is a relative unit. It is relative to the viewport width. 1vw is 1% of the viewport width. If the viewport width is 1000px, 1vw is 10px. If the viewport width is 2000px, 1vw is 20px.

```css
div {
    width: 50vw;
    /* It will take viewport width let assume it is 1000px then it will mulitiply by 50
    
        50vw = 500px
    */
}
```


### 4.6 vh
vh is a relative unit. It is relative to the viewport height. 1vh is 1% of the viewport height. If the viewport height is 1000px, 1vh is 10px. If the viewport height is 2000px, 1vh is 20px.

```css
div {
    height: 50vh;
    /* It will take viewport height let assume it is 1000px then it will mulitiply by 50
    
        50vh = 500px
    */
}
```
