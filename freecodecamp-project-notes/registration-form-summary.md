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
Step 18: link a `<label>` and its nested `<input>` using the `for` and `id`
         attributes, following accessibility best practices
Step 19: give each `<input>` an appropriate value to its `type` attribute
Step 20: add a submit button under the last `<fieldset>` (i.e. a `<input>`
         with its `type` attribute set to "submit" and its `value` attribute
         set to "Submit")
Step 21: add `required` attribute to each `<input>` in the first `<fieldset>`
         to make inputting these data compulsory for submission
Step 22: add custom validation to the password `<input>` by setting its
         `minlength` attribute to "8" to prevent passwords with less than eight
         characters being submitted
Step 23: introduce the topic of regex in the context of setting the pattern of
         the password submitted.
Step 24: add three `<label>` in the next `<fieldset>` (for inputting a different
         set of info)
Step 25: add an `<input>` with its `type` attribute set to "radio" within the
         first two `<label>`
Step 26: add an `<input>` with its `type` attribute set to "checkbox" within the
         third `<label>`
Step 27: add appropriate text after each `<input>` nested inside the `<label>`
Step 28: set `name` attribute of both radio buttons to "account-type"
Step 29: follow the same instructions in Step 18, but for the elements of the
         second `<fieldset>`
Step 30: wrap a `<a>` pair around the "terms and conditions" text in the third
         `<label>` in the second `<fieldset>` and link it to freeCodeCamp's
         terms and conditions page
Step 31:

Summary of lesson learned:
1. CSS units: `vh`, `rem`
2. It's a good practice to set the `margin` of `<body>` to 0 because some
   browsers add some margin by default.
3. Data from `<form>` can be sent via either a GET request as URL parameters
   or a POST request in the request body (see Step 12).
4. To allow one button of a group of radio buttons to be selected at a time, set
   set the `name` attribute of all of them to the same value.