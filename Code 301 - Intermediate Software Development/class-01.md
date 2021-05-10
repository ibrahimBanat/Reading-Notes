# Responsive Web Design

With the growth in mobile Internet usage comes the question of how to build websites suitable for all users.
With the growth in mobile Internet usage comes the question of how to build websites suitable for all users.

## Responsive Overview

Responsive web design is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop. Responsive web design is focused around providing an intuitive and gratifying experience for everyone. Desktop computer and cell phone users alike all benefit from responsive websites.

![Respomsive website at multiple screens](https://www.tothepointdesign.eu/images/services/responsive-website-design2.png)

## Flexible layouts

Responsive web design is broken down into three main components, including flexible layouts, media queries, and flexible media.

- Flexible layouts, is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width.
  Flexible grids are built using relative length units, most commonly percentages or em units. These relative lengths are then used to declare common grid property values such as width, margin, or padding.

      - Relative Viewport Lengths

          These new units include `vw`, `vh`, `vmin`, and vmax. Overall support for these new units isn’t great, but it is growing. In time they look to play a large roll in building responsive websites.

          1. `vw` (Viewports width)
          2. `vh` (Viewports height)
          1. `vmin` Minimum of the viewport’s height and width
          1. `vmax` Maximum of the viewport’s height and width

      Flexible layouts do not advocate the use of fixed measurement units, such as pixels or inches. Reason being, the viewport height and width continually change from device to device.

      The formula is based around taking the target width of an element and dividing it by the width of it’s parent element. The result is the relative width of the target element.

```
target ÷ context = result
```

<br>

- Flexible Grid

Using the flexible grid formula we can take all of the fixed units of length and turn them into relative units. In this example we’ll use percentages but em units would work equally as well. Notice, no matter how wide the parent container becomes, the section and aside margins and widths scale proportionally.

Taking the flexible layout concept, and formula, and reapplying it to all parts of a grid will create a completely dynamic website, scaling to every viewport size. For even more control within a flexible layout, you can also leverage the `min-width`, `max-width`, `min-height`, and max-height properties.

## Media Queries

There are a couple different ways to use media queries, using the `@media` rule inside of an existing style sheet, importing a new style sheet using the `@import` rule, or by linking to a separate style sheet from within the HTML document. Generally speaking it is recommend to use the `@media` rule inside of an existing style sheet to avoid any additional HTTP requests.

```
HTML

<!-- Separate CSS File -->
<link href="styles.css" rel="stylesheet" media="all and (max-width: 1024px)">
```

```
CSS
/* @media Rule */
@media all and (max-width: 1024px) {...}

/* @import Rule */
@import url(styles.css) all and (max-width: 1024px) {...}
```
