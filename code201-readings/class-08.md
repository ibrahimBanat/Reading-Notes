# Css Layout

we are going to look at
how to control where each element sits
on a page and how to create attractive
page layouts.

## Positioning Elements

CSS treats each HTML element as if it is in its
own box. This box will either be a block-level
box or an inline box.

- Block-level elements
    
    starts a new line, Elments like:
    ```
    <h1>
    <p>
    <ul>
    <li>
    ```
- Inline Elements

    flow between surrounding text
    ```
    <img>
    <b>
    <li>
    ```

## Containing Elements 

If one block-level element sits inside another
block-level element then the outer box is
known as the containing or parent element.

## Position of Elements

CSS has the following `positioning schemes` that allow you to control
the layout of a page: normal flow, relative positioning, and absolute
positioning. You specify the positioning scheme using the position
property in CSS. 

- Normal flow

    Every block-level element
    appears on a new line, causing
    each item to appear lower down
    the page than the previous one.

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
    of any surrounding elements.

To indicate where a box should be positioned, you may also need to use
`box offset` properties to tell the browser how far from the top or bottom
and left or right it should be placed.


- Fixed Positioning

    This is a form of absolute
    positioning that positions
    the element in relation to the
    browser window

- Floating Elements
    Floating an element allows
    you to take that element out
    of normal flow and position
    it to the far left or right of a
    containing box.


## Screen Sizes

Different visitors to your site will have different sized screens that show
different amounts of information, so your design needs to be able to
work on a range of different sized screens.

The size of a user's screen
affects how big they can open
their windows and how much
of the page they will see. There
are also an increasing number
of handheld devices.

## Fixed Width Layouts

Fixed width layout
designs do not
change size as the
user increases
or decreases
the size of their
browser window.

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
