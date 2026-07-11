## Make the menu work on small screens

Use JavaScript so the burger menu can show and hide the navigation links.

## Step 1

In the project file tab, open **responsive-navbar.js**.

## Step 2
Add click events for opening and closing the menu.

```javascript filename="responsive-navbar.js" line_numbers="true" line_number_start="1" line_highlights="15-16"
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
```

## Step 3
Add the **JavaScript** file to the top of each **HTML** page. The Wildlife page is shown below. You will also need to add this to **index.html** and **climate.html**.

```html filename="wildlife.html" line_numbers="true" line_number_start="53" line_highlights="54"
    </main>
    <script type="text/javascript" src="responsive-navbar.js"></script>
  </body>
</html>
```

## Step 4

In `style.css`, add a media query to change the navbar layout on small screens. This shows the burger menu and stacks the links when the screen is small.

```css filename="style.css" line_numbers="true" line_number_start="211" line_highlights="212-236"
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
```

## Now run your code
Make your browser window narrow, click the burger icon, and check that the links appear and disappear.
