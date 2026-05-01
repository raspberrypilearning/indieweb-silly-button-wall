<h2 class="c-project-heading--task">Challenge: add three more cursed buttons</h2>

Copy the pattern you already know to fill the wall with three extra buttons and three extra sounds.

<h2 class="c-project-heading--explainer">Make this change</h2>

Open `index.html` and `style.css`. The extra MP3 files are already in the project folder, so you only need to add the new buttons, the new audio elements, the extra click handlers, and your own styles.

<div class="c-project-code">

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 18
line_highlights: 19-27
---
        <button class="silly-button glitter" type="button">refresh flop era</button>
        <button class="silly-button oops" type="button">oops all screenshots</button>
        <button class="silly-button forbidden" type="button">cringe portal</button>
      </section>

      <audio id="drama-sound" src="drama.mp3" preload="auto"></audio>
      <audio id="nope-sound" src="nope.mp3" preload="auto"></audio>
      <audio id="panic-sound" src="panic.mp3" preload="auto"></audio>
      <audio id="glitter-sound" src="glitter.mp3" preload="auto"></audio>
      <audio id="oops-sound" src="oops.mp3" preload="auto"></audio>
      <audio id="forbidden-sound" src="forbidden.mp3" preload="auto"></audio>
--- /code ---

</div>

<div class="c-project-code">

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 45
line_highlights: 51-59
---
      document.querySelector(".glitter").addEventListener("click", function () {
        playButtonSound("#glitter-sound");
      });

      document.querySelector(".oops").addEventListener("click", function () {
        playButtonSound("#oops-sound");
      });

      document.querySelector(".forbidden").addEventListener("click", function () {
        playButtonSound("#forbidden-sound");
      });
--- /code ---

</div>

<div class="c-project-tip">

<h3>Tip</h3>

<p>`glitter` looks good with a sugary gradient, rounded corners, and a tiny jump on hover.</p>

<p>`oops` looks good with a wonky border radius, a messier orange colour, and a sideways skew on hover.</p>

<p>`forbidden` looks good with warning stripes, pale text, and a small scale-up when hovered.</p>

<p>Copy one of your earlier listener blocks if you want each extra button to play its own MP3.</p>

<p><a href="https://www.google.com/search?q=web+colour+picker" target="_blank" rel="noopener noreferrer">Open the Google web colour picker in a new tab</a> if you want help choosing colours.</p>

</div>

## Now run your code

If you add the extra buttons and style them, your wall should feel much closer to the six-button version shown below.

<div class="c-project-output">
  <img src="images/step_4_output.png" alt="Expected project output after step 4 showing the full six-button panic wall.">
</div>
