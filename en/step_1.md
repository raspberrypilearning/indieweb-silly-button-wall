<h2 class="c-project-heading--task">Build the fake drama button</h2>

Add one loud button to the wall, then make it jump and squeal when clicked.

<h2 class="c-project-heading--explainer">Make this change</h2>

Use the empty button wall in `index.html` as your starting point. Add the button HTML, give it its own CSS class, and make it play `drama.mp3`.

## Step 1

Put this button inside `<section class="button-wall">`, then add the matching audio element underneath the section.

<div class="c-project-code">

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 11
line_highlights: 15-18
---
    <main class="button-stage">
      <p class="eyebrow">Recovered profile controls // cached at 1:43am</p>
      <h1>PROFILE PANIC BUTTON WALL</h1>
      <p>Three cursed profile buttons are waiting for one truly awful mood.</p>
      <section class="button-wall">
        <button class="silly-button drama" type="button">start fake drama</button>
      </section>

      <audio id="drama-sound" src="drama.mp3" preload="auto"></audio>
    </main>
--- /code ---

</div>

## Step 2

Open `style.css` and add these rules underneath `.silly-button`.

<div class="c-project-code">

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 99
line_highlights: 99-107
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
--- /code ---

</div>

## Step 3

Go back to `index.html` and add this code inside `<script>` so the button plays its sound when someone clicks it.

<div class="c-project-code">

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 18
line_highlights: 19-27
---
    <script>
      function playButtonSound(soundId) {
        const sound = document.querySelector(soundId);
        sound.currentTime = 0;
        sound.play();
      }

      document.querySelector(".drama").addEventListener("click", function () {
        playButtonSound("#drama-sound");
      });
    </script>
--- /code ---

</div>

## Now run your code

The bright pink button should hop when you hover over it and play a short dramatic sound when you click it.

<div class="c-project-output">
  <img src="images/step_1_output.png" alt="Expected project output after step 1 showing one styled fake drama button inside the panic panel.">
</div>
