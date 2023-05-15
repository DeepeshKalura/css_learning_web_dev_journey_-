# CSS Learning
## 3. Lesson Three: Color

There are may types of clour we can use in CSS. The most common are:
1. Color name
    ```css
    body{
        color: red;
    }
    ```
In this case, the color name is `red`. There are many color names we can use. like `black`, `green`.

Note: Color names are not good pratice to use. Because they are not very descriptive, and does not generate a color pallet well.


2. Hexadecimal
    ```css
    body{
        color: #ff0000;
    }
    ```
In this case, the color is `#ff0000`. Hexadecimal colors are a combination of 6 characters. The first two characters are the red value, the second two are the green value, and the last two are the blue value. Each character can be a number from 0 to 9, or a letter from A to F. The lowest value is 0, and the highest value is FF. The lowest value is no color, and the highest value is full color. So, `#ff0000` is full red, `#00ff00` is full green, and `#0000ff` is full blue.

Note: It is good for beginners to use hexadecimal colors. Because they are easy to understand, and they are very common.

3. RGB
    ```css
    body{
        color: rgb(255, 0, 0);
    }
    ```
In this case the color is `rgb(255, 0, 0)`. RGB colors are a combination of 3 numbers. The first number is the red value, the second number is the green value, and the last number is the blue value. Each number can be a number from 0 to 255. The lowest value is 0, and the highest value is 255. The lowest value is no color, and the highest value is full color. So, `rgb(255, 0, 0)` is full red, `rgb(0, 255, 0)` is full green, and `rgb(0, 0, 255)` is full blue.

Note: RGB colors are very common. They are easy to understand, and they are very flexible. It is good for beginners to use RGB colors.

4. RGBA
    ```css
    body{
        color: rgba(255, 0, 0, 0.5);
    }
    ```
In this case the color is `rgba(255, 0, 0, 0.5`. RGBA colors are combinationof 4 numbers. The first number is the red value, the secnd number is gren value, the third number is blue value and the last number is the alpha value (I even called as opacity value). Each number can be a number from 0 to 255, except last value it goes from 0 to 1. The lowest value is 0, and the highest value is 255. The lowest value is no color, and the highest value is full color. So, `rgba(255, 0, 0, 0.5)` is half red, `rgba(0, 255, 0, 0.5)` is half green, and `rgba(0, 0, 255, 0.5)` is half blue.

5. HSL
    ```css
    body{
        color: hsl(0, 100%, 50%);
    }
    ```
In this case the color is `hsl(0, 100%, 50%)`. HSL colors are combination of 3 numbers. The first number is the hue value, the second number is the saturation value, and the last number is the lightness value. The hue value can be a number from 0 to 360. The saturation value can be a number from 0% to 100%. The lightness value can be a number from 0% to 100%. The lowest value is 0, and the highest value is 360. The lowest value is no color, and the highest value is full color. So, `hsl(0, 100%, 50%)` is full red, `hsl(120, 100%, 50%)` is full green, and `hsl(240, 100%, 50%)` is full blue.

6. HSLA
    ```css
    body{
        color: hsla(0, 100%, 50%, 0.5);
    }
    ```
In this case the color is `hsla(0, 100%, 50%, 0.5)`. HSLA colors are combination of 4 numbers. The first number is the hue value, it goes from 0 to 360 like represent in color wheel. The second number is suturation value, it goes from 0% to 100%. The third number is lightness value, it goes from 0% to 100%. The last number is alpha value, it goes from 0 to 1. The lowest value is 0, and the highest value is 360. The lowest value is no color, and the highest value is full color. So, `hsla(0, 100%, 50%, 0.5)` is half red, `hsla(120, 100%, 50%, 0.5)` is half green, and `hsla(240, 100%, 50%, 0.5)` is half blue.

These are the mostly theory part of color. Now we will see some practical part of color.

### Color Pallet

In web application or general we have to use colour with the combination of other colour. So, we have to use colour pallet. There are many colour pallet we can use. But the most common colour pallet are:
1. Background and Text Color
    ```css
    body{
        background-color: #ffffff;
        color: #000000;
    }
    ```
In this case the background color is `#ffffff` and the text color is `#000000`. The background color is white and the text color is black. This is the most common color pallet. Because it is easy to read.

So, to check the contract between then we use [contrast ratio](https://coolors.co/contrast-checker/112a46-acc8e5). In this website we can check the contract between two color. The contract ratio should be 4.5:1. If the contract ratio is less than 4.5:1 then it is not good for reading.



