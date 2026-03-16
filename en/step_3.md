<h2 class="c-project-heading--task">Add hero images</h2>

--- task ---
Add a big “hero image” at the top of a page to show what it’s about.
--- /task ---

--- task ---
Open `climate.html` and add a hero image `<div>` underneath the header.

<div class="c-project-code">

--- code ---
---
language: html
filename: climate.html
line_numbers: true
line_number_start: 10
line_highlights: 24
---
<body>
  <header>
    <nav class="navigation-header">
      <div class="nav-items">
        <a href="index.html">Home</a>
        <a href="wildlife.html">Wildlife</a>
        <a class="active" href="climate.html">Climate</a>
      </div>
      <div class="burger">
        <span id="openHam">&#9776;</span>
        <span id="closeHam">&#x2716;</span>
      </div>
    </nav>
  </header>
  <div class="hero-image climate"></div>
  <main>
--- /code ---

</div>

--- /task ---

--- task ---
**Test:** Run the Climate page and check a large image appears near the top of the page.
--- /task ---