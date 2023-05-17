# CSS Learning

## Lesson Twenty-Two: Animations

### Animations
- CSS animations are used to create animations on HTML elements.
- CSS animations are created using the `@keyframes` rule.
- The `@keyframes` rule contains the property changes and their values during the animation.
- The `animation-name` property is used to specify the name of the animation.
- The `animation-duration` property is used to specify the duration of the animation.
- The `animation-timing-function` property is used to specify the speed of the animation.
- The `animation-delay` property is used to specify the delay before the animation starts.
- The `animation-iteration-count` property is used to specify the number of times the animation should be played.
- The `animation-direction` property is used to specify the direction of the animation.
- The `animation-fill-mode` property is used to specify the style applied to the element when the animation is not playing.
- The `animation-play-state` property is used to specify whether the animation is running or paused.
- The `animation` shorthand property is used to specify all the animation properties in one declaration.
``` css
@keyframes my-animation {
  0% {
    background-color: red;
  }
  50% {
    background-color: blue;
  }
  100% {
    background-color: green;
  }
}
```
