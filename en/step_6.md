<h2 class="c-project-heading--task">Add hover animations</h2>

Make your facts appear when you hover over a card.

--- task ---

Open `style.css` and hide fact text until the user hovers.

<div class="c-project-code">

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 114
line_highlights: 132-134,138
---
.fact {
  font-size: 100%;
  color: var(--fact-text-colour);
  background-color: var(--fact-background);
  height: 100%;
  margin: 0;
  display: flex;
  flex-wrap: wrap;
  align-content: center;
  padding: 0 5px 0 5px;
  opacity: 0;
  transition: 0.4s ease-in-out;
}

/* Fact hover */
.fact:hover {
  opacity: 1;
}
--- /code ---

</div>

--- /task ---

--- task ---

**Test:** Hover over a card and check the fact text fades in.

--- /task ---