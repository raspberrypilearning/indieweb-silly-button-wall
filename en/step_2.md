<h2 class="c-project-heading--task">Build the aura button</h2>

Add a second button with its own weird shape and its own rude little sound.

## Step 1

Add this extra button inside `<section class="button-wall">`, then add the matching audio element underneath the first one.

<div class="c-project-code">

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 15
line_highlights: 17-20
---
      <section class="button-wall">
        <button class="silly-button drama" type="button">start fake drama</button>
        <button class="silly-button nope" type="button">delete my aura</button>
      </section>

      <audio id="drama-sound" src="drama.mp3" preload="auto"></audio>
      <audio id="nope-sound" src="nope.mp3" preload="auto"></audio>
--- /code ---

</div>

## Step 2

Open `style.css` and add these rules underneath `.drama:hover`.

<div class="c-project-code">

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 109
line_highlights: 109-117
---
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
--- /code ---

</div>

## Step 3

Go back to `index.html` and add this extra click handler underneath the first one.

<div class="c-project-code">

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 25
line_highlights: 29-31
---
      document.querySelector(".drama").addEventListener("click", function () {
        playButtonSound("#drama-sound");
      });

      document.querySelector(".nope").addEventListener("click", function () {
        playButtonSound("#nope-sound");
      });
    </script>
--- /code ---

</div>

## Now run your code

You should now have two buttons. The blue one should twist slightly on hover and play its own blunt little sound when clicked.

<div class="c-project-output">
  <img src="images/step_2_output.png" alt="Expected project output after step 2 showing two styled buttons in the panic panel.">
</div>
