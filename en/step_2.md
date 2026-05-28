<h2 class="c-project-heading--task">Create a navigation bar</h2>

## Step 1
Open `index.html` and create a navigation bar so visitors can move between pages.

<div class="c-project-code">

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 11
line_highlights: 12-21
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
    </header>
--- /code ---

</div>

## Step 2

Open `wildlife.html` and `climate.html` and add the same code.

## Step 3

Add `class="active"` to the link for the file you are editing.

## Now run your code
Click the navbar links, and check that you can open **Home**, **Wildlife**, and **Climate**.

<div class="c-project-output">

![output screenshot](images/step3.png)

</div>
