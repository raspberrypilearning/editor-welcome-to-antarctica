<h2 class="c-project-heading--task">Create a navigation bar</h2>

--- task ---

Open `index.html` and create a navigation bar so visitors can move between pages.

<div class="c-project-code">

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 11
line_highlights: 12-22
---
    <header>
      <nav>
        <div class="nav-items"> 
          <a class="active" href="index.html">Home</a>
          <a href="wildlife.html">Wildlife</a>
          <a href="climate.html">Climate</a>
        </div>
        <div class="burger">
          <span id="openHam">&#9776;</span>
          <span id="closeHam">&#x2716;</span>
        </div>
      </nav>
      <div class="hero-image home"></div>
    </header>
--- /code ---

</div>

--- /task ---

--- task ---

Do the same for the other pages: `wildlife.html` and `climate.html`.

Add the `active` class attribute to the page you are working on.

--- /task ---

--- task ---

**Test:** Click Run, then click the links in your navbar to check you can open **Home**, **Wildlife**, and **Climate**.

--- /task ---