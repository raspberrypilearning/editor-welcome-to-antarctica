<h2 class="c-project-heading--task">Create a climate grid</h2>

--- task ---

Open `climate.html` and set up the fact cards.

Add the `fact-holder` class attribute to the `<div>`.

Add a `fact-card` and a background image class to each `<span>` element.

Add the `fact` class attribute to each paragraph.

<div class="c-project-code">

--- code ---
---
language: html
filename: climate.html
line_numbers: true
line_number_start: 29
line_highlights: 30-49
---
  <section>
    <h1>Hover on the cards below to learn about the climate in Antarctica</h1>
    <div class="fact-holder">
      <span class="fact-card temperature">
        <p class="fact">
          Antarctica is the coldest continent on Earth. The average temperature in the interior is -57°C, during winter it can reach -90°C.
        </p>
      </span>
      <span class="fact-card sunburn">
        <p class="fact">
          You can get sunburn on Antarctica as the snow reflects nearly all of the sun's ultraviolet rays. You may not feel the heat, but you still need to keep your skin safe from the rays.
        </p>
      </span>
      <span class="fact-card ice">
        <p class="fact">
          Antarctica's ice sheet is, on average, 1.6km thick and covers about 98% of the continent. This ice sheet is nearly 90% of the entire world’s ice!
        </p>
      </span>
      <span class="fact-card rainfall">
        <p class="fact">
          Technically, Antarctica is a desert because it is so dry there. The average annual precipitation on the coast is just 166mm.
        </p>
      </span>
    </div>
  </section>
    
--- /code ---

</div>

--- /task ---

--- task ---

Open `style.css`.

Add the `fact-holder-wildlife` selector to the `style.css` file.

<div class="c-project-code">

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 104
line_highlights: 105-110
---

/* Fact holder - wildlife */
.fact-holder-wildlife {
  display: grid;
  height: 70vh;
  grid-template-rows: 1fr 1fr 1fr;
  grid-template-columns: 2fr 3fr;
}

--- /code ---

</div>

--- /task ---

--- task ---

**Test:** Run the Wildlife page and check you can hover the cards to reveal the facts.

--- /task ---