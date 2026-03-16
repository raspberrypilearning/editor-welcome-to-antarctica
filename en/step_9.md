<h2 class="c-project-heading--task">Make grids responsive</h2>

Change your grids so the cards are easy to read on small screens.

--- task ---

Open `style.css` and add responsive grid rules inside your media query.

<div class="c-project-code">

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 211
line_highlights: 237-257
---
@media screen and (max-width: 768px) {

  .fact-holder {
    height: 100vh;
    grid-template-rows: 25% 25% 25% 25%;
    grid-template-columns: 100%;
  }

  .fact-holder-wildlife {
    height: 140vh;
    grid-template-rows: 1fr 1fr 1fr 1fr 1fr;
    grid-template-columns: 1fr;
  }

  .penguins {
    grid-row-start: 1;
    grid-row-end: 3;
  }

  .orcas {
    grid-column-start: 1;
    grid-column-end: 2;
  }
}
--- /code ---

</div>

--- /task ---

--- task ---

**Test:** Make your browser narrow and check the cards stack vertically and are easier to read.

--- /task ---