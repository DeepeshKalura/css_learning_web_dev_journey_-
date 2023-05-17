# CSS Learning

## Lesson 16: Image

### 1. Image
Image is a very important part of a website. It can make the website more vivid and beautiful. In this lesson, we will learn how to use image in CSS.
```css
img {
    width: 100px;
    height: 100px;
}
```
The above code will set the width and height of the image to 100px. 

There are two types of images we can use in CSS: background-image and content-image.

### 2. Background-image
We can use background-image to set the background image of an element. The background image will be repeated by default. We can use background-repeat to set the repeat mode of the background image. The value of background-repeat can be no-repeat, repeat-x, repeat-y, repeat. The default value is repeat. The following code will set the background image of the body element to bg.png, and the background image will not be repeated.
```css
body {
    background-image: url(bg.png);
    background-repeat: no-repeat;
}
```
We can also use background-position to set the position of the background image. The value of background-position can be left top, left center, left bottom, right top, right center, right bottom, center top, center center, center bottom. The default value is left top. The following code will set the background image of the body element to bg.png, and the background image will not be repeated. The background image will be displayed in the center of the body element.
```css
body {
    background-image: url(bg.png);
    background-repeat: no-repeat;
    background-position: center center;
}
```
We can also use background-attachment to set whether the background image scrolls with the page. The value of background-attachment can be scroll, fixed, local. The default value is scroll. The following code will set the background image of the body element to bg.png, and the background image will not be repeated. The background image will be displayed in the center of the body element. The background image will not scroll with the page.
```css
body {
    background-image: url(bg.png);
    background-repeat: no-repeat;
    background-position: center center;
    background-attachment: fixed;
}
```
We can also use background-size to set the size of the background image. The value of background-size can be length, percentage, cover, contain. The default value is auto. The following code will set the background image of the body element to bg.png, and the background image will not be repeated. The background image will be displayed in the center of the body element. The background image will not scroll with the page. The background image will be displayed in the center of the body element.
```css
body {
    background-image: url(bg.png);
    background-repeat: no-repeat;
    background-position: center center;
    background-attachment: fixed;
    background-size: cover;
}
```
### 3. Content-image
We can use content-image to set the content image of an element. The content image will not be repeated by default. We can use content-repeat to set the repeat mode of the content image. The value of content-repeat can be no-repeat, repeat-x, repeat-y, repeat. The default value is no-repeat. The following code will set the content image of the body element to bg.png, and the content image will not be repeated.
```css
body {
    content-image: url(bg.png);
    content-repeat: no-repeat;
}
```
We can also use content-position to set the position of the content image. The value of content-position can be left top, left center, left bottom, right top, right center, right bottom, center top, center center, center bottom. The default value is left top. The following code will set the content image of the body element to bg.png, and the content image will not be repeated. The content image will be displayed in the center of the body element.
```css
body {
    content-image: url(bg.png);
    content-repeat: no-repeat;
    content-position: center center;
}
```
We can also use content-size to set the size of the content image. The value of content-size can be length, percentage, cover, contain. The default value is auto. The following code will set the content image of the body element to bg.png, and the content image will not be repeated. The content image will be displayed in the center of the body element. The content image will be displayed in the center of the body element.
```css
body {
    content-image: url(bg.png);
    content-repeat: no-repeat;
    content-position: center center;
    content-size: cover;
}
```
There are more amazing things about image. Which we can learn when we does lots of practice.

Note: There is site in which caniuse.com we can check the browser support for the CSS properties.

like background clip property is not supported by the IE browser.
```css
body {
    background-image: url(bg.png);
    background-repeat: no-repeat;
    background-position: center center;
    background-attachment: fixed;
    background-size: cover;
    background-clip: content-box;
}
```
but in google chrome it is supported.
see in website https://caniuse.com/
