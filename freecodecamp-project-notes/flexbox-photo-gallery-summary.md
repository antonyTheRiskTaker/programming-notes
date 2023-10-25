# Photo Gallery Project (CSS Flexbox)

## Walkthrough

Step 1: set up boilerplate code by adding `DOCTYPE` declaration, `<html>` (with
        `lang` attribute set to "en"), `<head>` and `<body>`
Step 2: add a viewport `<meta>` (to make the page mobile-friendly) and another
        `<meta>` for setting the character encoding for the web page
Step 3: add `<title>` and `<link>` (for adding CSS to the page)
Step 4: (now turn to `<body>`) add `<header>` (with a `header` class) and nest
        a `<h1>` inside it
Step 5: below the `<header>`, add a `<div>` gallery container and nest nine
        `<img>` inside it
Step 6: fill the `<img>` with links to cat photos
Step 7: in the stylesheet, target `.gallery` and `<img>` and set their `width`,
        `border` and `padding` to appropriate values
Step 8: (VERY IMPORTANT!) introduce `box-sizing` CSS property
Step 9: (VERY IMPORTANT!) explain what does the `border-box` value of the
        `box-sizing` CSS property do
Step 10: remove the `.gallery` and `img` rules
Step 11: target `.gallery img` and set the `width`, `max-wdith` and `height`
         properties to appropriate values
Step 12: (VERY IMPORTANT!) remove the `margin` from the `<body>`, set its
         `font-family` and `background-color` properties
Step 13: style the `.header` element and set its `text-align`, `text-transform`,
         `padding`, `background`, `color` and `border-bottom` properties to
         appropriate values
Step 14: introduce a one-dimension CSS layout flexbox and the concepts of
         flex container and flex item
Step 15: introduce the `flex-direction` CSS flexbox property
Step 16: introduce the `flex-wrap` CSS flexbox property
Step 17: introduce the `justify-content` CSS flexbox property
Step 18: introduce the `align-items` CSS flexbox property
Step 19:

## Summary of lesson learned

1. New CSS properties learned: `box-sizing`
2. The difference between the `content-box` and `border-box` values of the
   `box-sizing` CSS property (See steps 8 and 9).
3. CSS good practice No.1: target all HTML elements and set their `box-sizing`
   property to `border-box` (BUT WHY? For building responsive web pages?).
4. CSS good practice No.2: remove `margin` from `<body>` and set other page-wide
   properties in the `.body` rule.
