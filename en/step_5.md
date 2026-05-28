<h2 class="c-project-heading--task">Different hero images</h2>

Each page should have its own hero image that represents its content!

## Step 1

In `style.css`, find the `/* Hero image - wildlife */` comment and the code underneath it.

<div class="c-project-code">

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 90
line_highlights: 91-93
---
/* Hero image - wildlife */
.wildlife {
  background-image: url('antarctic-penguins.jpg');
}
--- /code ---

</div>

## Step 2

In **wildlife.html** add the `hero-image` class.

<div class="c-project-code">

--- code ---
---
language: html
filename: wildlife.html
line_numbers: true
line_number_start: 23
line_highlights: 24
---
    </header>
    <div class="hero-image wildlife"></div>
    <main>
--- /code ---

</div>

## Step 3

In **style.css**, find the `/* Hero image - climate */` comment and add the following code underneath it.

<div class="c-project-code">

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 95
line_highlights: 96-98
---
/* Hero image - climate */
.climate {
  background-image: url('antarctic-daytime.jpg');
}
--- /code ---

</div>

## Step 4

In **climate.html**, add the new `climate` class.

<div class="c-project-code">

--- code ---
---
language: html
filename: climate.html
line_numbers: true
line_number_start: 22
line_highlights: 23
---
  </header>
  <div class="hero-image climate"></div>
  <main>
--- /code ---

</div>

## Now run your code
Check that a large image appears near the top of each page.

<div class="c-project-output">

![output screenshot](images/step6.png)

</div>
