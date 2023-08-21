Step 1: create a `<!DOCTYPE html>` declaration to begin the project
Step 2: add a `<html>` with an `lang` attribute set to "en"; below the
        declaration
Step 3: add a `<head>` and `<body>` inside the `<html>`
Step 4: add a `<meta>` with a `charset` attribute set to "UTF-8" and a title of
        'Registration Form' (`<title>`)
Step 5: add `<link>` inside `<head>` to link a CSS stylesheet (styles.css) to
        the HTML page
Step 6: add `<h1>` within the `<body>`
Step 7: below `<h1>` heading, add a `<p>` with text to encourage users to
        register
Step 8: introduce `vh` unit for CSS styling and the concept of viewport
Step 9: set the `margin` of `<body>` to '0' to remove the horizontal scroll bar
Step 10: set the `background-color` and `color` on `<body>` to specified values
Step 11: add a `<form>` after the `<p>`
Step 12: introduce the `method` attribute of `<form>`
Step 13: add three `<fieldset>` inside the `<form>`
Step 14: add four `<label>` inside the first `<fieldset>`
Step 15: add text to the four `<label>` to prompt users to input their first
         names, last names, email, and to create passwords
Step 16: introduce the unit of `rem`
Step 17: nest an `<input>` within each `<label>`
Step 18: link a `<label>` and its nested `<input>` using the `for` attribute,
         following accessibility best practices
Step 19: give each `<input>` an appropriate value to its `type` attribute
Step 20: add a submit button under the last `<fieldset>` (i.e. a `<input>`
         with its `type` attribute set to "submit" and its `value` attribute
         set to "Submit")
Step 21: add `required` attribute to each `<input>` in the first `<fieldset>`
         to make inputting these data compulsory for submission
Step 22:

Summary of lesson learned:
1. CSS units: `vh`, `rem`
2. It's a good practice to set the `margin` of `<body>` to 0 because some
   browsers add some margin by default.
3. Data from `<form>` can be sent via either a GET request as URL parameters
   or a POST request in the request body (see Step 12).