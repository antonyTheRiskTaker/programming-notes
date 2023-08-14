Step 1: create a `<!DOCTYPE html>` declaration, followed by an `<html>`
Step 2: inside the `<html>`, create a `<head>` and `<body>`
Step 3: add `<title>` within `<head>` and explain its purpose
Step 4: add `<meta>` within `<head>` and set its `charset` attribute to "utf-8"
Step 5: add `<meta>` within `<head>` with `name` and `content`
        attributes set to appropriate values, so that the page looks the same
        on all devices
Step 6: add `<h1>` within `<body>` with the name of the project
Step 7: link a CSS stylesheet to the HTML page
Step 8: style `<h1>`'s `text-align` property to 'center'
Step 9: add a `<div>` with its class set to `container` under `<h1>`
Step 10: within the container `<div>`, add another `<div>` and set its class as
         `marker`
Step 11: add `background-color: red;` to the `.marker` selector
Step 12: set `.marker`'s `height` and `width` to '25px' and '200px' respectively
Step 13: introduce `margin` as the shorthand for `margin-top`, `margin-bottom`,
         `margin-left` and `margin-right`
Step 14: add two more `<div>` with its class set to `container`
Step 15: in the `.container` CSS rule, set `margin` to '10px auto'
Step 16: show how to make a HTML element take multiple classes
Step 17: remove the `background-color` property and its value from the `.marker`
         CSS rule
Step 18: create a new CSS rule that targets the class `one` and set its
         `background-color` property to 'red'
Step 19: add classes `two` and `three` to the respective `<div>`s
Step 20: create two CSS rules `.two` and `.three` and set their
         `background-color` to 'green' and 'blue' respectively
Step 21: introduce two colour models and the CSS `rgb` function
Step 22: explain what a function is and how rgb colour works
Step 23: use the `rgb()` to create green and blue colours for the `.two` and
         `.three` CSS rules
Step 24: in the `.two` CSS rule, set the green value in the `rgb()` to '127'
         to lower its intensity
Step 25: in the `.container` CSS rule, use the `padding` property to add '10px'
         of top and bottom padding, and set the left and right padding to '0'
Step 26: introduce primary colours in the RGB colour model
Step 27: in the `.container` rule, set the red, green and blue values to the
         max of '255'
Step 28: introduce secondary colours in the RGB colour model
Step 29: mix pure green and pure blue to create the cyan colour using `rgb()` in 
         the `.two` CSS rule
Step 30: mix pure red and pure blue to create the magenta colour using `rgb()`
         in the `.three` CSS rule
Step 31: introduce tertiary colours in the RGB colour model
Step 32: mix green and cyan to create spring green using `rgb()` in the `.two`
         CSS rule
Step 33: mix magenta and blue to create violet using `rgb()` in the `.three` CSS
         rule
Step 34: create chartreuse green, azure and rose colours in the `.one`, `.two`
         and `.three` CSS rules respectively
Step 35: set the `background-color` of `.one`, `.two` and `.three` CSS rules
         to pure black using `rgb()`
Step 36: introduce the concepts of hues (similar colours) and complementary
         colours in a colour wheel
Step 37: introduce the practice of choosing one colour as dominant colour, and
         its complementary colour as an accent to bring attention to certain
         content on the page
Step 38: set the `background-color` to black and red in the `.one` and `.two`
         CSS rules respectively
Step 39: set the `background-color` to black in the `.two` CSS rule
Step 40: remove the `background-color` property and value in the `h1` CSS rule
Step 41: in the first marker `<div>`, change the class `one` to `red`
Step 42: update the `.one` CSS rule to target the `red` class
Step 43: update `rgb()` in the `.red` CSS rule so that the red value is at the
         max
Step 44: change the class `two` and `three` to `green` and `blue` in their
         respective colour marker `<div>`
Step 45: update the CSS selectors `.two` and `.three` so that they target the
         new `green` and `blue` classes respectively
Step 46: introduce hexadecimal values as a way to apply colour to HTML elements
         with CSS
Step 47: set the intensity of green by setting the green value of the hex
         colour to '7f'
Step 48: introduce the HSL colour model
Step 49: introduce gradient (colour transition) and the `linear-gradient`
         CSS function
Step 50: explain the syntax of `linear-gradient()`
Step 51: in the `linear-gradient()`, use the `rgb()` to set the first colour
         argument to pure red
Step 52: set the second colour argument to pure green, using the `rgb()`
Step 53: set the third colour argument to pure blue
Step 54: introduce colour-stops in `linear-gradient()`
Step 55: set the `gradientDirection` argument to '180deg' for the
         `linear-gradient()`
Step 56: set the colour stop for red to '0%', green to '50%', and blue to '100%'
Step 57: update the first colour argument in the `linear-gradient()`:
         red -> 122, green -> 74, and blue -> 14
Step 58: modify the second colour argument: red -> 245, green -> 62, and blue ->
         113
Step 59: modify the third colour argument: red -> 162, green -> 27, and blue ->
         27
Step 60: in the `.green` CSS rule, change the `background-color` property to
         `background`
Step 61: set the `background` property to `linear-gradient()` and set the
         function's `gradientDirection` to '180deg'. The first colour argument
         is '#55680D'
Step 62: set the second colour argument to '#71f53e'
Step 63: set the third colour argument to '#116c31'
Step 64: `linear-gradient()` places colours evenly along the gradient line by
         default
Step 65: `linear-gradient()` ranges colours from top to bottom (along a 180
         degree line) by default
Step 66: in the `.blue` CSS rule, change the `background-color` property to
         `background`
Step 67: use `linear-gradient()` and pass in `hsl()` with values of '186',
         '76%' and '16%' for hue, saturation and lightness respectively
Step 68: pass in `hsl(223, 90%, 60%)` as the second colour argument
Step 69: pass in `hsl(240, 56%, 42%)` as the third colour argument
Step 70: build a marker sleeve for the red marker by creating a new `<div>` with
         a class of `sleeve` and nesting it inside the red marker `<div>`
Step 71: create a new CSS rule targeting the `sleeve` class and set its
         `width` to '110px' and `height` to '25px'
Step 72: set the `.sleeve`'s `background-color` to 'white'
Step 73: introduce the `opacity` CSS property
Step 74: introduce another way to set the opacity of an element with 
         `alpha channel`
Step 75: introduce the CSS `rgba` function
Step 76: add another `<div>` with a `cap` class before the sleeve `<div>`
         in order to push the latter to the right side of the colour bar
Step 77: create a CSS rule targetting the `cap` class and set its `width` and
         `height` to '60px' and '25px' respectively
Step 78: create a new CSS rule targetting both `cap` and `sleeve`, and set
         their `display` to 'inline-block'
Step 79: properties of an HTML element's border can be controlled separately,
         e.g. `border-left-width` (a new CSS property introduced)
Step 80: introduce `border-left-style` CSS property
Step 81: introduce `border-left-color` CSS property
Step 82: introduce `border-left` shorthand CSS property
Step 83: switch `border-left`'s style value to 'double'
Step 84: set `border-left`'s colour value to pure black with 75% opacity using
         `rgba()`
Step 85: add caps and sleeves to other markers
Step 86: introduce `box-shadow` CSS property
Step 87: position the shadow of the red marker on the opposite side by updating
         the offsetX and offsetY values of `.red`'s `box-shadow` CSS property
Step 88:         

Summary of lesson learned:
1. New CSS properties learned: `opacity`, `border-left-width`,
   `border-left-style`, `border-left-color`
2. New CSS functions learned: `rgb()`, `hsl()`, `linear-gradient()`, `rgba()`
3. "utf-8" is a universal character set that includes almost every character
   from all human languages.
4. A HTML element can take multiple classes, however the styles of the first
   class in the list can be overridden by later classes.
5. `margin` CSS property syntax: `margin: [top] [right] [bottom] [left];`
6. `border-left` CSS property syntax: `border-left: [width] [style] [colour];`
7. `box-shadow` CSS property syntax: `box-shadow: [offsetX] [offsetY] [colour]`