<h2 class="c-project-heading--task">Add hero images</h2>

Add a big 'hero image' at the top of a page to show what it’s about.

--- task ---

Add a hero image `<div>` underneath the header on each page.

<div class="c-project-code">

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 23
line_highlights: 24
---
  </header>
  <div class="hero-image"></div>
  <main>
--- /code ---

--- /task ---

--- task ---

In `style.css`, add a new selector for the `hero-image` class.

Instead of adding an `<img>` element to the HTML, you can use the CSS `background-image` property to add your image. 

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 73
line_highlights: 74-79
---

/* Hero image - homepage */
.hero-image {
  min-height: 50vh; /* 50% of the visible area of the page */
  background-image: url('antarctic-lights.jpg'); 
  background-size: cover;
  background-position: center;
}

--- /code ---

</div>

--- /task ---

--- task ---

**Test:** Check a large image appears near the top of the page.

--- /task ---