<h2 class="c-project-heading--task">Style the button stage</h2>

You will turn the page shell into a proper stage for your ridiculous buttons.

Still in `style.css`, add the `.button-stage` rule underneath `p`.

<div class="c-project-tip">

<h3>Tip</h3>

<p>`padding` changes how much breathing room the panel has inside it.</p>

<p>`border` changes how heavy and loud the panel outline feels.</p>

<p>`box-shadow` changes how much the panel seems to lift off the page.</p>

<p>`border-radius` changes whether the panel corners feel sharp or rounded.</p>

</div>

<div class="c-project-code">

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 28
line_highlights: 30-39
---
}

.button-stage {
  width: min(720px, 100%);
  padding: 28px;
  border: 6px solid #1d1230;
  border-radius: 24px;
  background: rgba(255, 255, 255, 0.88);
  box-shadow:
    0 0 0 8px #ffffff,
    0 18px 0 #1d1230;
}
--- /code ---

</div>

<h2 class="c-project-heading--task">Test</h2>

The heading, paragraph, and buttons should now sit inside one big bright panel.

<div class="c-project-output">
  <img src="images/step_3_output.png" alt="Observed project output after this step.">
</div>
