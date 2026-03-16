<h2 class="c-project-heading--task">Add responsive CSS</h2>

Show the burger menu and stack the links when the screen is small.

--- task ---

Open `style.css` and add a media query to change the navbar layout on small screens.

<div class="c-project-code">

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 211
line_highlights: 212-235
---
/* Media query */
@media screen and (max-width: 768px) {
  
  .burger {
    display: flex;
    cursor: pointer;
  }

  .burger #closeHam {
    display: none;
  }

  .nav-items {
    display: none;
    flex-direction: column;
    align-items: center;
    position: absolute;
    right: 0;
    top: 58px;
    background-color: var(--nav-colour);
    width: 100%;
    height: calc(100vh - 58px);
    padding-top: 60px;
    gap: 10vh;
  }
}
--- /code ---

</div>

--- /task ---

--- task ---

**Test:** Shrink your browser and check the burger icon appears (and the links don’t take up space until you open the menu).

--- /task ---