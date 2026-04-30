<h2 class="c-project-heading--task">Add the cursed control header</h2>

Add the visible header inside `<main class="button-stage">` so the page stops looking empty.

<h2 class="c-project-heading--explainer">Make this change</h2>

Open `index.html`. The starter file has an empty `<main>` element, so add the eyebrow, the main heading, and the short paragraph inside it.

<div class="c-project-code">

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 1
line_highlights: 10-14
---
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>PROFILE PANIC BUTTON WALL</title>
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
    <main class="button-stage">
      <p class="eyebrow">Recovered profile controls // cached at 1:43am</p>
      <h1>PROFILE PANIC BUTTON WALL</h1>
      <p>Six cursed profile buttons are waiting for one truly awful mood.</p>
    </main>
  </body>
</html>
--- /code ---

</div>

## Now run your code

You should see the recovered profile header inside the panel instead of a blank box.

<div class="c-project-output">
  <img src="images/step_1_output.png" alt="Expected project output after step 1 showing the profile control header inside the panel.">
</div>
