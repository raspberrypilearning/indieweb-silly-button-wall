<h2 class="c-project-heading--task">Make it play drama.mp3</h2>

Add one click handler so the drama button plays its sound.

<h2 class="c-project-heading--explainer">Make this change</h2>

In `index.html`, add this code inside `<script>` so the button plays `drama.mp3` when someone clicks it.

<div class="c-project-code">

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 21
line_highlights: 22-30
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

The bright pink button should still hop on hover and now play a short dramatic sound when you click it.

<div class="c-project-output">
  <img src="images/step_3_output.png" alt="Expected project output after step 3 showing one styled fake drama button inside the wall panel.">
</div>
