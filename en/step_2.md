## Create a navigation bar

## Step 1
Open `index.html` and create a navigation bar so visitors can move between pages.

```html filename="index.html" line_numbers="true" line_number_start="11" line_highlights="12-21"
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
```

## Step 2

Open `wildlife.html` and `climate.html` and add the same code.

## Step 3

Add `class="active"` to the link for the file you are editing.

## Now run your code
Click the navbar links, and check that you can open **Home**, **Wildlife**, and **Climate**.

![output screenshot](images/step3.png)
