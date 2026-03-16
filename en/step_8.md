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

**Test:** Make your browser window narrow and click the burger icon — the links should appear and disappear.

--- /task ---