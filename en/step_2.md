<h2 class="c-project-heading--task">Change the font</h2>

--- task ---

Import a Google font to style the fonts on your pages.

Open `defaults.css`.

You can find it in the file list next to `style.css` and your HTML files.

Place this `@import` statement at the top of your file.

<div class="c-project-code">

--- code ---
---
language: css
filename: defaults.css
line_numbers: true
line_number_start: 1
line_highlights: 2
---

/* Import a font */
@import url('https://fonts.googleapis.com/css2?family=Orbitron&display=swap');

--- /code ---

</div>

--- /task ---

--- task ---

Create a new variable inside the `:root` selector, called `--body-font` and set the new Orbitron font.

<div class="c-project-code">

--- code ---
---
language: css
filename: defaults.css
line_numbers: true
line_number_start: 4
line_highlights: 7
---

:root {
  --body-background: #ece8ef;
  --body-text-colour: #000500;
  --body-font: "Orbitron", sans-serif;

--- /code ---

</div>

--- /task ---

--- task ---

Add the `font-family` property inside the body selector and set it to the new `--body-font` variable you just created.

<div class="c-project-code">

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 1
line_highlights: 11
---
body {
  background-color: var(--body-background);
  color: var(--body-text-colour);
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  width: 100%;
  min-height: 100vh; /* Make the content fill the page so the footer is at the bottom */
  display: flex;
  flex-direction: column;
  font-family: var(--body-font);
}
--- /code ---

</div>

--- /task ---

--- task ---

**Test:** Click Run to see your new font!

--- /task ---

<div class="c-project-output">

![output screenshot](images/step2.png)

</div>
