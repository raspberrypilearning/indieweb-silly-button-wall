<h2 class="c-project-heading--task">Give it terminally bad taste</h2>

Change the custom properties at the top of `style.css` so the page gets darker, louder, and more chaotic.

<h2 class="c-project-heading--explainer">Make this change</h2>

Open `style.css` and edit the values inside `:root`. These custom properties control the page background, the panel colours, the main accent colours, the border size, the font, and the width of the panel.

<div class="c-project-tip">

<h3>Tip</h3>

<p>Pick colours that feel like cached profile glitter, fake warning stickers, or a control panel that should not exist.</p>

<p>Small value changes can make the whole page feel more sugary, more dramatic, or more suspicious.</p>

<p><a href="https://www.google.com/search?q=web+colour+picker" target="_blank" rel="noopener noreferrer">Open the Google web colour picker in a new tab</a> if you want help choosing colours.</p>

</div>

<div class="c-project-code">

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 1
line_highlights: 2-15
---
/* Change these values to give the control panel terminally bad taste. */
:root {
  --page-bg: #120014;
  --ink: #26001b;
  --panel-bg: #ffd8f2;
  --accent: #7eeeff;
  --accent-hot: #ff73c6;
  --accent-acid: #c3ff63;
  --accent-warning: #ffe45a;
  --accent-mess: #ff9b54;
  --shadow-color: #170011;
  --border-size: 5px;
  --corner-size: 18px;
  --body-font: Verdana, Geneva, sans-serif;
  --stage-width: 35rem;
}
--- /code ---

</div>

## Now run your code

The page should still work the same way, but it should now look more like a cursed profile control panel.

<div class="c-project-output">
  <img src="images/step_3_output.png" alt="Expected project output after step 3 showing darker colours and louder control-panel styling.">
</div>
