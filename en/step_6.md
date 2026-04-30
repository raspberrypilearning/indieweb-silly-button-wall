<h2 class="c-project-heading--task">Make every button suspicious</h2>

Give each button its own strange shape, colour, and hover effect.

<h2 class="c-project-heading--explainer">Make this change</h2>

Stay in `style.css` and add the individual button styles underneath `.silly-button`.

<div class="c-project-tip">

<h3>Tip</h3>

<p>`background` sets the button colours or gradients.</p>

<p>`border-radius` changes each button shape from tidy to weird.</p>

<p>`box-shadow` changes how raised, flat, or bent each button looks.</p>

<p>`transform` changes how each button reacts on hover.</p>

</div>

<div class="c-project-code">

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 99
line_highlights: 99-172
---
.drama {
  background: var(--accent-hot);
  border-radius: 28px 10px 28px 10px;
  box-shadow: 0 8px 0 #9d1e61;
}

.drama:hover {
  transform: translateY(-4px) rotate(-2deg);
  box-shadow: 0 12px 0 #9d1e61;
}

.nope {
  background: var(--accent);
  border-radius: 14px;
  box-shadow: 8px 8px 0 var(--ink);
}

.nope:hover {
  background: #46d9ff;
  transform: rotate(3deg);
  letter-spacing: 0.08em;
}

.panic {
  background: var(--accent-warning);
  border-radius: 999px;
  box-shadow: 0 0 0 6px #ff8b38;
}

.panic:hover {
  transform: scale(1.06);
  box-shadow: 0 0 0 10px #ff8b38;
}

.glitter {
  background: linear-gradient(135deg, #fffef8, #ff9de0, #8dfff6);
  border-radius: 24px;
  box-shadow: 0 8px 0 var(--ink);
}

.glitter:hover {
  transform: translateY(-4px);
  background: linear-gradient(135deg, #fff2a1, #ff73c6, #63f3ff);
}

.oops {
  background: var(--accent-mess);
  border-radius: 18px 30px 14px 30px;
  box-shadow: -8px 8px 0 var(--ink);
}

.oops:hover {
  transform: skew(-4deg, -1deg);
  background: #ff6d4f;
}

.forbidden {
  background:
    repeating-linear-gradient(
      -45deg,
      var(--accent-warning) 0 14px,
      var(--ink) 14px 28px
    );
  border-radius: 12px;
  color: #fff8cf;
  text-shadow: 2px 2px 0 rgba(38, 0, 27, 0.7);
  box-shadow: 0 8px 0 var(--accent-hot);
}

.forbidden:hover {
  transform: translateY(-2px) scale(1.03);
  box-shadow: 0 12px 0 var(--accent-hot);
  filter: saturate(1.15);
}
--- /code ---

</div>

## Now run your code

Hover over the wall and each button should react in its own ridiculous way.

<div class="c-project-output">
  <img src="images/step_6_output.png" alt="Expected project output after step 6 showing the final suspicious button wall with different button styles.">
</div>
