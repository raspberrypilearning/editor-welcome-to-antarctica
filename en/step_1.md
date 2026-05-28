<h2 class="c-project-heading--task">Change the font</h2>

Import a Google font to style the fonts on your pages.

## Step 1

Click on the project files tab and open `defaults.css`.

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

## Step 2

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
  --nav-colour: #33658a;
--- /code ---

</div>

## Step 3

Open `style.css` and add the `font-family`.

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

## Now run your code
Check that the page uses the new font.

<div class="c-project-output">

![output screenshot](images/step2.png)

</div>
