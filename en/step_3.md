## Style the navigation bar

In `style.css`, find the `/* Nav bar */` comment.

Add the styles in the code under each comment.

> [!TIP]
>
> Run your code when you add each bit of code and see how it changes the site.

```css filename="style.css" line_numbers="true" line_number_start="37" line_highlights="45,49-52,55-59,62-64,67-70,73-79"
/* Nav bar */
nav {
  padding: 0 15px;
  height: 60px;
  font-size: 22px;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: var(--nav-colour);
}

/* Nav items */
.nav-items {
  display: flex;
  gap: 100px;
}

/* Nav bar links */
.nav-items > a {
  color: var(--nav-items-colour);
  text-decoration: none;
  transition: 0.4s ease-in-out;
}

/* Nav links hover */
.nav-items > a:hover {
  color: var(--nav-items-active);
}

/* Nav links active */
.nav-items .active {
  color: var(--nav-items-active);
  pointer-events: none;
}

/* Burger menu */
.burger {
  display: none;
  font-size: 20px;
  font-weight: 800;
  color: var(--burger-colour);
  margin-left: auto;
}
```

## Now run your code
Check that the navbar is styled and the current page link looks active.

![output screenshot](images/step4.png)
