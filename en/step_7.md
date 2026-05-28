<h2 class="c-project-heading--task">Add hover animations</h2>

In `style.css`, add this code to hide the facts until the user hovers over them. 

<div class="c-project-code">

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 120
line_highlights: 130-131, 135-137
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

## Now run your code
Hover over a card and check that the fact text fades in.

<div class="c-project-output">

![output screenshot](images/step8.png)

</div>
