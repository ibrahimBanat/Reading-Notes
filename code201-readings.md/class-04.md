# Html

## Links

Links are the defining feature of the web
because they allow you to move from
one web page to another — enabling the
very idea of browsing or surfing.


### Writing Links

Links are created using the `<a>` element. Users can click on anything
between the opening `<a>` tag and the closing `</a>` tag. You specify
which page you want to link to using the href attribute.

### Opening Links in a New Window

- target

    ```
    <a href="http://www.imdb.com" target="_blank">
    Internet Movie Database</a> (opens in new window)
    ```

### Linking to a Specific Part of the Same Page

At the top of a long page
you might want to add a list
of contents that links to the
corresponding sections lower
down. Or you might want to add
a link from part way down the
page back to the top of it to save
users from having to scroll back
to the top.

``` 
<h1 id="top">Film-Making Terms</h1>
<a href="#arc_shot">Arc Shot</a><br />
<a href="#interlude">Interlude</a><br />
<a href="#prologue">Prologue</a><br /><br />
<h2 id="arc_shot">Arc Shot</h2>
<p>A shot in which the subject is photographed by an
 encircling or moving camera</p>
<h2 id="interlude">Interlude</h2>
<p>A brief, intervening film scene or sequence, not
 specifically tied to the plot, that appears
 within a film</p>
<h2 id="prologue">Prologue</h2>
<p>A speech, preface, introduction, or brief scene
 preceding the the main action or plot of a film;
 contrast to epilogue</p>
<p><a href="#top">Top</a></p>

```
## Summary 

- Links are created using the `<a>` element.
- The `<a>` element uses the href attribute to indicate
the page you are linking to.
- If you are linking to a page within your own site, it is
best to use relative links rather than qualified URLs.
- You can create links to open email programs with an
email address in the "to" field.
- You can use the id attribute to target elements within
a page that can be linked to.


## Layout

### Controlling the Position of Elements

CSS has the following positioning schemes that allow you to control
the layout of a page: normal flow, relative positioning, and absolute
positioning. You specify the positioning scheme using the position
property in CSS. You can also float elements using the float property.

- Normal flow

    Every block-level element
    appears on a new line, causing
    each item to appear lower down
    the page than the previous one.
    Even if you specify the width
    of the boxes and there is space
    for two elements to sit side-byside, they will not appear next
    to each other. This is the default
    behavior (unless you tell the
    browser to do something else)

- Relative Positioning

    This moves an element from the
    position it would be in normal
    flow, shifting it to the top, right,
    bottom, or left of where it
    would have been placed. This
    does not affect the position of
    surrounding elements; they stay
    in the position they would be in
    in normal flow.

- Absolute positioning

    This positions the element
    in relation to its containing
    element. It is taken out of
    normal flow, meaning that it
    does not affect the position
    of any surrounding elements
    (as they simply ignore the
    space it would have taken up).
    Absolutely positioned elements
    move as users scroll up and
    down the page.


### Creating Multi-Column layouts

Many web pages use multiple
columns in their design. This
is achieved by using a `<div>`
element to represent each
column. The following three CSS
properties are used to position
the columns next to each other: 

- width

    This sets the width of the
    columns

- float

    This positions the columns next
    to each other.

- margin

    This creates a gap between the
    columns.
    A two-column layout like the one
    shown on this page would need
    two `<div>` elements, one for the
    main content of the page and
    one for the sidebar.

## Summary
- `<div>` elements are often used as containing elements
to group together sections of a page.

- Browsers display pages in normal flow unless you
specify relative, absolute, or fixed positioning.

- The float property moves content to the left or right
of the page and can be used to create multi-column
layouts. (Floated items require a defined width.)

- Pages can be fixed width or liquid (stretchy) layouts.

- Designers keep pages within 960-1000 pixels wide,
and indicate what the site is about within the top 600
pixels (to demonstrate its relevance without scrolling).

- Grids help create professional and flexible designs.

- CSS Frameworks provide rules for common tasks.

- You can include multiple CSS files in one page.

# Funtions 

Browsers require very detailed instructions about what
we want them to do. Therefore, complex scripts can run
to hundreds (even thousands) of lines. Programmers use
functions, methods, and objects to organize their code. 

## What is the function 

Functions let you group a series of statements together to perform a
specific task. If different parts of a script repeat the same task, you can
reuse the function (rather than repeating the same set of statements).

### A basic function 


``` 
var msg = 'Sign up to recive out newsletter for 10% off!';

function updateMessage() {
    var el = document.getElementById('message');
    el.textContent = msg;
}
updateMessage();
```

### Declearing a function

To create a function, you give it a name and then write the statements needed to achibe it's task inside the curly braces. This known as a **function declaration**.
![](img/fucntion.PNG)


### Calling a function 

Having declared the function, you can excute all of the statements between it's curly braces with just one line of cide.
this is known as calling the function.

![](img/invoke.PNG)

### Declaring a Functions that need information
SomeTimes a function needs specific information to perform it's task.

In such cases, when you declare the function you give it **arameter**.

![](img/param.PNG)

- Arguments as values:
    ```
    getArea(3,5);
    ```

- Arguments as Variables 
    ```
    wallWidth = 3;
    wallheight = 5; 
    getArea(wallWidth, wallHieght);
    ```

### Getting a single value out of funtion 

Some function return information to the code that called them. For example, when they perform a calculation, they return the result.

```
function calcualteArea(width, height) {
    var area = width * height;
    return area;
}
var wallOne = calculateArea(3, 5);
var wallTwo = calculateArea(8, 5);
```


### Getting a multiple values out of function 

function can return more than one value using array. 
for example, this function calculates the area and the voulme of a box. 

``` 
function getSize(width, height, depth) { 
    var area = width * height;
    var volume = width * height * depth;
    var sizes = [area, volume];
}
var areaOne = getSize(3, 2, 3)[0];
var volumeOne = getSize(3, 2, 3)[1];