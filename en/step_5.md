<h2 class="c-project-heading--task">Make the buttons loud</h2>

Add one shared button style so every button gets bigger, bolder, and more obviously clickable.

<h2 class="c-project-heading--explainer">Make this change</h2>

Stay in `style.css` and add the `.silly-button` rule underneath `.button-wall`.

<div class="c-project-tip">

<h3>Tip</h3>

<p>`padding` changes how chunky each button feels.</p>

<p>`font-size` and `font-weight` change how loud the labels feel.</p>

<p>`transition` makes the hover effects feel smoother later.</p>

</div>

<div class="c-project-code">

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 86
line_highlights: 86-97
---
.silly-button {
  padding: 18px 16px;
  border: 4px solid var(--ink);
  color: var(--ink);
  background: #fffefb;
  font: inherit;
  font-size: 1.1rem;
  font-weight: 900;
  line-height: 1.1;
  cursor: pointer;
  transition: transform 0.18s ease, box-shadow 0.18s ease, background 0.18s ease, letter-spacing 0.18s ease, filter 0.18s ease;
}
--- /code ---

</div>

## Now run your code

The buttons should now look much bigger and bolder, even though they still share one plain style.

<div class="c-project-output">
  <img src="images/step_5_output.png" alt="Expected project output after step 5 showing the bigger shared button style.">
</div>
