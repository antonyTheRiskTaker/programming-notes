# Nutrition Label Project (CSS Typography)

## Walkthrough

1. add `<h1>` (with appropriate text) in the `<body>` in the HTML boilerplate
2. add `<p>` under the `<h1>` and give it some text
3. add another `<p>` for serving size
4. add two `<link>` for Google font and your own stylesheet
5. create the `body` selector and set its `font-family` to the Google font
6. create the `html` selector and set its `font-size` to "16px"
7. wrap the previous `<h1>` and `<p>` in a `<div>` (with `label` class)
8. target `.label` and set its `border` to appropriate values
9. set `.label`'s `width` to an appropriate value to create white space around
   the label
10. set the `margin` and `padding` attributes of the `.label` to appropriate
    values
11. set all elements' `box-sizing` property to "border-box" in order to include
    padding and border to their sizes
12. introduce CSS property `font-weight`
13. center `h1`
14. set `h1`'s `margin` to appropriate values
15. remove all margins of `p`
16. create a `<div>` and set its `class` attribute to "divider"
17. create a `.divider` selector and set its `border-bottom` and `margin` to
    appropriate values
18. introduce `letter-spacing` CSS property
19. give the second `<p>` a class of "bold"
20. create a `.bold` selector, set its `font-weight` to an appropriate value,
    and remove the `font-weight` declaration from the `h1` ruleset
21. set `<h1>`'s class attribute to "bold" to make the text bold
22. wrap the text "2/3 cup (55g)" in a `<span>`
23. make `<p>` flexbox elements and set its `justify-content` to "space-between"
24. wrap everything within the `.label` element in a `<header>`
25. update the `h1` selector to be `header h1` to specifically target the `<h1>`
    within the new `<header>`
26. create a new `<div>` and set its class attribute to "divider large"
27. create `.large` and `.large .medium` selectors and set their `height` and
    `background-color` properties to appropriate values
28. set `.large .medium`'s `border` to "0"
29. create a new `<div>` and set its class to "calories-info"
30. within the calories-info `<div>`, create another `<div>` and `<h2>`
31. create a `.small-text` selector and set the `font-size` to "0.85rem"
32. create a `.calories-info h2` selector and remove all margins
33. add a new `<p>` below the `.small-text` element and a new `<span>`
    below the `.left-container` element
34. create a `.calories-info` selector and set its `display`, `justify-content`
    and `align-items` to appropriate values (hint: we are creating a flex
    container)
35. create a `.left-container p` selector and set its `margin`, `font-size` and
    `font-weight` to appropriate values
36. create a `.calories-info span` selector and set its `font-size` and
    `font-weight` to appropriate values
37. set `margin` of the `.calories-info span` selector to appropriate values
38. add a new `<div>` below the `.calories-info` element and add its class
    attribute to "divider" and "medium"
39. create a `.medium` selector and set its `height` to an appropriate value
40. create a `<div>`, nest a `<p>` within it, and give appropriate class names
    to both elements
41. move the text "% Daily Value *" to the right of the label using
    `justify-content`
42. add a new divider after the `<p>` within the daily value `<div>`
43. under the divider `<div>`, add a `<p>` and three `<span>` that wrap the
    content of the `<p>`
44. below the `<p>` with the "Total Fat" text, create a new `<p>` with
    appropriate text, and within the `<p>` wrap part of the text with a `<span>`
45. give the "Saturated Fat" `<p>` a class set to "indent"
46. create an `.indent` selector and set its `margin-left` to "1em"
47. create a `daily-value p` selector and set its `border-bottom` to appropriate
    values
48. add "no-divider" to the class attribute of the `<p>` with the texts
    "% Daily Value *" and "Saturated Fat 1g 5%"
49. introduce the `:not` pseudo-selector
50. add another `.divider` `<div>` under the second `.no-divider` `<p>`
51. introduce the `<i>` element
52. create another `.divider` `<div>` under the `<p>` created in step 52
53. after the last `.divider` `<div>`, add another `<p>` for cholesterol
    content, wrap appropriate parts of the text in `<span>`, and assign "bold"
    to the class attribute of some of the `<span>`
54. add another `<p>` for sodium content, wrap appropriate parts of the text in
    `<span>`, and assign "bold" to the class attribute of some of the `<span>`
55. add another `<p>` for carbohydrate content, wrap appropriate parts of the
    text in `<span>`, and assign "bold" to the class attribute of some of the
    `<span>`
56.

## Summary of lesson learned

1. New CSS properties learned: `font-weight`, `letter-spacing`
2. New CSS pseudo-selector learned: `:not`
3. New HTML elements learned: `<i>`
