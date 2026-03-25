<h2 class="c-project-heading--task">Make the menu work on small screens</h2>

Use JavaScript so the burger menu can show and hide the navigation links.

--- task ---

Open `responsive-navbar.js` and add click events for opening and closing the menu.

<div class="c-project-code">

--- code ---
---
language: javascript
filename: responsive-navbar.js
line_numbers: true
line_number_start: 1
line_highlights: 15-16
---
let openHam = document.querySelector('#openHam');
let closeHam = document.querySelector('#closeHam');
let navigationItems = document.querySelector('.nav-items');

const burgerEvent = (navigation, close, open) => { 
    if (navigation == "none"){
        navigationItems.style.removeProperty("display");
    } else {
        navigationItems.style.display = navigation;
    }
    closeHam.style.display = close;
    openHam.style.display = open;
}

openHam.addEventListener('click', () => burgerEvent("flex", "block", "none"));
closeHam.addEventListener('click', () => burgerEvent("none", "none", "block"));
--- /code ---

</div>

--- /task ---

--- task ---

Also add the **JavaScript** file to each page. 

<div class="c-project-code">

--- code ---
---
language: html
filename: wildlife.html
line_numbers: true
line_number_start: 53
line_highlights: 54
---
    </main>
    <script type="text/javascript" src="responsive-navbar.js"></script>
  </body>
</html>

--- /code ---

</div>

--- /task ---

--- task ---

Show the burger menu and stack the links when the screen is small.

Open `style.css` and add a media query to change the navbar layout on small screens.

<div class="c-project-code">

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 211
line_highlights: 212-236
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

**Test:** Make your browser window narrow and click the burger icon. The links should appear and disappear.

--- /task ---
