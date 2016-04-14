# Color Me Angular
Learn ngRoute with colors.

This lab uses [148 Built-In CSS Color Names](https://gist.github.com/nathanallen/22dbc2c0dbe1b6d2d197721ec9eeab61#file-color_names-json).

## The Challenge
Your goal is to create an angular front-end that displays information about css colors:

* When a user navigates to "/", they should see a list of all 148 css colors.
* When a user navigates to "/000000", they should see information about hexadecimal color `#000000`, otherwise known as "Black".
* Color names should link to their approriate `show` page.
* The `colors/show.html` should have a convenient "back" button that returns the user to the home page.

## Setup
Clone this repo.

We will be using a new development server called `budo` for this project.

```bash
npm install -g budo
```

Run the server:
```
budo -P --host=localhost --open
```

## ngRoute Setup
TODO

## Bonuses
* **Semantic Routes**: Create separate routes for `/color/name/:name` and `color/hex/:hex`, but have them route to the same show page.
    * Since there are only 148 named colors in css, and 16^6 (16,777,216) hex colors, not every show page can have a color name in the title. Can you accomodate for this?
* **Color Picker**: Add an HTML5 colorpicker (input type 'color') to `colors/show.html`.
    * Set its initial value to the hex value of the show page.
    * Stretch: when the user changes their color selection, redirect them to the appropriate show page.
* **Sort the Colors**: Add a [filter](https://docs.angularjs.org/api/ng/filter/filter) to `colors/index.html` that sorts colors by name, alphabetically.
    * Next, add a button to the index page that, on click...
        * sorts colors by `name`.
        * sorts colors by `hex`.
        * Stretchy Stretch: toggles between ascending/descending sort order with every click.

## Resources
* Built-in Directives
    - [`ngRepeat`](https://docs.angularjs.org/api/ng/directive/ngRepeat)
        + [`filter`](https://docs.angularjs.org/api/ng/filter/filter)
    - [`ngHref`](https://docs.angularjs.org/api/ng/directive/ngHref)
    - [`ngStyle`](https://docs.angularjs.org/api/ng/directive/ngStyle)
* [`ngRoute` Module](https://docs.angularjs.org/api/ngRoute)
    - [`ngView` directive](https://docs.angularjs.org/api/ngRoute/directive/ngView)
    - [`$routeProvider`](https://docs.angularjs.org/api/ngRoute/provider/$routeProvider)
    - [`$locationProvider`](https://docs.angularjs.org/api/ng/provider/$locationProvider)
    - [`$routeParams`](https://docs.angularjs.org/api/ngRoute/service/$routeParams)
