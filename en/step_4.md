<h2 class="c-project-heading--task">Arrange the button wall</h2>

You will turn the button section into a neat grid instead of one awkward stack.

Still in `style.css`, add the `.button-wall` rule underneath `.button-stage`.

<div class="c-project-tip">

<h3>Tip</h3>

<p>`grid-template-columns` changes how many buttons can fit across each row.</p>

<p>`gap` changes the space between the buttons.</p>

<p>`margin-top` changes how far the wall sits below the heading text.</p>

</div>

<div class="c-project-code">

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 39
line_highlights: 41-46
---
}

.button-wall {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
  gap: 18px;
  margin-top: 22px;
}
--- /code ---

</div>

<h2 class="c-project-heading--task">Test</h2>

The buttons should now sit in a proper wall instead of stacking in one narrow line.

<div class="c-project-output">
  <img src="images/step_4_output.png" alt="Observed project output after this step.">
</div>
