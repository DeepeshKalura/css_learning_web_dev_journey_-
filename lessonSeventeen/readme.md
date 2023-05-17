# CSS learning

## Lesson 17: Media Queries

Task 1 We have t study about the the css framework to make the website responsive. We have to study about the bootstrap and the tailwirl css. Just check the breakpoint of the bootstrap and the tailwirl css

### Media Queries

Media queries are a popular technique for delivering a tailored style sheet to different devices. You can use it to target different screen sizes, orientations, and resolution.

### Media Types
Media types describe the general category of a device. For example, you can use media types to define a style for screen and print media types. The following table lists the media types that are defined in the CSS specification:
- all - Used for all media type devices
- print - Used for printers
- screen - Used for computer screens, tablets, smart-phones etc.
- speech - Used for screenreaders that "reads" the page out loud

### Media Features
Media features describe specific characteristics of the user agent, output device, or environment. You can use media features to apply styles based on the following characteristics:
- Width and height of the browser
- Width and height of the output device
- Orientation (is the tablet/phone in landscape or portrait mode?)
- Resolution

### Media Queries Syntax
Media queries consist of a media type and can, optionally, contain one or more expressions, which resolve to either true or false.
```css
@media not|only mediatype and (expressions) {
    CSS-Code;
}
```
- not: Negates the query, so that it returns true if the query would otherwise return false.
- only: Returns true if the device is a browser and the user has specified that they do not want paged media.
- and: Returns true if both the expressions on the left and right are true.
- ,: Returns true if either the expression on the left or the right is true.

### Media Queries Example
```css
@media only screen and (max-width: 500px) {
    body {
        background-color: lightblue;
    }
}
```
### Media Queries - Logical Operators
Logical operators can be used in media queries to express very specific conditions.
- and: If both the conditions separated by and are true, the styles inside the curly braces are applied.
- or: If either of the conditions separated by or is true, the styles inside the curly braces are applied.
- not: If the condition after not is false, the styles inside the curly braces are applied.

### Media Queries - Width and Height
The following example will change the background color of the page to lightblue if the width of the browser window is less than 500px:
```css
@media only screen and (max-width: 500px) {
    body {
        background-color: lightblue;
    }
}
```
The following example will change the background color of the page to lightblue if the width of the browser window is more than 500px:
```css
@media only screen and (min-width: 500px) {
    body {
        background-color: lightblue;
    }
}
```
The following example will change the background color of the page to lightblue if the width of the browser window is between 500px and 800px:
```css
@media only screen and (min-width: 500px) and (max-width: 800px) {
    body {
        background-color: lightblue;
    }
}
```
The following example will change the background color of the page to lightblue if the width of the browser window is less than 500px or more than 800px:
```css
@media only screen and (max-width: 500px), (min-width: 800px) {
    body {
        background-color: lightblue;
    }
}
```
The following example will change the background color of the page to lightblue if the height of the browser window is less than 500px:
```css
@media only screen and (max-height: 500px) {
    body {
        background-color: lightblue;
    }
}
```
The following example will change the background color of the page to lightblue if the height of the browser window is more than 500px:
```css
@media only screen and (min-height: 500px) {
    body {
        background-color: lightblue;
    }
}
```
The following example will change the background color of the page to lightblue if the height of the browser window is between 500px and 800px:
```css
@media only screen and (min-height: 500px) and (max-height: 800px) {
    body {
        background-color: lightblue;
    }
}
```
The following example will change the background color of the page to lightblue if the height of the browser window is less than 500px or more than 800px:
```css
@media only screen and (max-height: 500px), (min-height: 800px) {
    body {
        background-color: lightblue;
    }
}
```
### Media Queries - Orientation
The following example will change the background color of the page to lightblue if the orientation of the browser is in landscape mode:
```css
@media only screen and (orientation: landscape) {
    body {
        background-color: lightblue;
    }
}
```
The following example will change the background color of the page to lightblue if the orientation of the browser is in portrait mode:
```css
@media only screen and (orientation: portrait) {
    body {
        background-color: lightblue;
    }
}
```
### Media Queries - Resolution
The following example will change the background color of the page to lightblue if the resolution of the screen is 72dpi or more:
```css
@media only screen and (min-resolution: 72dpi) {
    body {
        background-color: lightblue;
    }
}
```
The following example will change the background color of the page to lightblue if the resolution of the screen is 300dpi or more:
```css
@media only screen and (min-resolution: 300dpi) {
    body {
        background-color: lightblue;
    }
}
```
The following example will change the background color of the page to lightblue if the resolution of the screen is between 72dpi and 300dpi:
```css
@media only screen and (min-resolution: 72dpi) and (max-resolution: 300dpi) {
    body {
        background-color: lightblue;
    }
}
```
The following example will change the background color of the page to lightblue if the resolution of the screen is less than 72dpi or more than 300dpi:
```css
@media only screen and (max-resolution: 72dpi), (min-resolution: 300dpi) {
    body {
        background-color: lightblue;
    }
}
```
### Media Queries - Aspect Ratio
The following example will change the background color of the page to lightblue if the aspect ratio of the browser window is 16/9:
```css
@media only screen and (aspect-ratio: 16/9) {
    body {
        background-color: lightblue;
    }
}
```
The following example will change the background color of the page to lightblue if the aspect ratio of the browser window is 4/3:
```css
@media only screen and (aspect-ratio: 4/3) {
    body {
        background-color: lightblue;
    }
}
```
The following example will change the background color of the page to lightblue if the aspect ratio of the browser window is between 16/9 and 4/3:
```css
@media only screen and (aspect-ratio: 16/9) and (aspect-ratio: 4/3) {
    body {
        background-color: lightblue;
    }
}
```
The following example will change the background color of the page to lightblue if the aspect ratio of the browser window is less than 16/9 or more than 4/3:
```css
@media only screen and (aspect-ratio: 16/9), (aspect-ratio: 4/3) {
    body {
        background-color: lightblue;
    }
}
```
### Media Queries - Pixel Density
The following example will change the background color of the page to lightblue if the pixel density of the screen is 1.5 or more:
```css
@media only screen and (min-device-pixel-ratio: 1.5) {
    body {
        background-color: lightblue;
    }
}
```
The following example will change the background color of the page to lightblue if the pixel density of the screen is 2 or more:
```css
@media only screen and (min-device-pixel-ratio: 2) {
    body {
        background-color: lightblue;
    }
}
```
The following example will change the background color of the page to lightblue if the pixel density of the screen is between 1.5 and 2:
```css
@media only screen and (min-device-pixel-ratio: 1.5) and (max-device-pixel-ratio: 2) {
    body {
        background-color: lightblue;
    }
}
```
The following example will change the background color of the page to lightblue if the pixel density of the screen is less than 1.5 or more than 2:
```css
@media only screen and (max-device-pixel-ratio: 1.5), (min-device-pixel-ratio: 2) {
    body {
        background-color: lightblue;
    }
}
```
