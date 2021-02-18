## Images 

There are many reasons why you might
want to add an image to a web page: you
might want to include a logo, photograph,
illustration, diagram, or chart.

### Choosing Images for Your Site 

A picture can say a thousand words, and great
images help make the difference between an
average-looking site and a really engaging one.

### Storing Images on Your Site

If you are building a site from scratch, it is good
practice to create a folder for all of the images
the site uses.


### Adding Images

`<img>` 
To add an image into the page
you need to use an `<img>`
element. This is an empty
element (which means there is
no closing tag). It must carry the
following two attributes:

- `src`

    This tells the browser where
    it can find the image file. This
    will usually be a relative URL
    pointing to an image on your
    own site.

- `alt`

    This provides a text description
    of the image which describes the
    image if you cannot see it.

- `title`

    You can also use the title
    attribute with the `<img>` element
    to provide additional information
    about the image.

### Where to Place Images in Your Code

Where an image is placed
in the code will affect how it
is displayed. Here are three
examples of image placement
that produce different results:

1. before a paragraph 

    The paragraph starts on a new
    line after the image.
2. inside the start of a paragraph

    The first row of text aligns with
    the bottom of the image.

3. in the middle of a
    paragraph

### Rules for Creating Images

1. Save images in
the right format

    Websites mainly use images in
    jpeg, gif, or png format. If you
    choose the wrong image
    format then your image might
    not look as sharp as it should
    and can make the web page
    slower to load.

2. Save images at
the right size

    You should save the image at
    the same width and height it will
    appear on the website. 

3. Use the correct
resolution

    Computer screens are made up
    of dots known as pixels. Images
    used on the web are also made
    up of tiny dots. Resolution refers
    to the number of dots per inch,
    and most computer screens only
    show web pages at 72 pixels
    per inch.

### Figure and Figure Caption

- `<figure>`

    Images often come with
    captions. HTML5 has introduced
    a new `<figure>` element to
    contain images and their caption
    so that the two are associated.

- `<figcaption>`

    The `<figcaption>` element has
    been added to HTML5 in order
    to allow web page authors to add
    a caption to an image.

## Summary

- The `<img>` element is used to add images to a
web page.

- You must always specify a src attribute to indicate the
source of an image and an alt attribute to describe the
content of an image.

- You should save images at the size you will be using
them on the web page and in the appropriate format.

- Photographs are best saved as JPEGs; illustrations or
logos that use flat colors are better saved as GIFs.

## colors

Color can really bring your pages to life.

## Foreground Color (color)

The color property allows you
to specify the color of text inside
an element. You can specify any
color in CSS in one of three ways:

``` 
/* color name */
h1 {
color: DarkCyan;}
/* hex code */
h2 {
color: #ee3e80;}
/* rgb value */
p {
color: rgb(100,100,90);}
```
- rgb values 

    These express colors in terms
of how much red, green and
blue are used to make it up. For
example: `rgb(100,100,90)`.

- hex codes 

    These are six-digit codes that
    represent the amount of red,
    green and blue in a color,
    preceded by a pound or hash #
    sign. For example: `#ee3e80`.

- color names 

    There are 147 predefined color
names that are recognized
by browsers. For example:
`DarkCyan`. 

### Background color 

``` 
body {
background-color: rgb(200,200,200);}
h1 {
background-color: DarkCyan;}
h2 {
background-color: #ee3e80;}
p {
background-color: white;}
```
CSS treats each HTML element
as if it appears in a box, and the
background-color property
sets the color of the background
for that box.

You can specify your choice of
background color in the same
three ways you can specify
foreground colors: RGB values,
hex codes, and color names
(covered on the next page).
If you do not specify a
background color, then the
background is transparent. 

### Understanding Color
 
Every color on a computer screen is created by mixing amounts of red,
green, and blue. To find the color you want, you can use a color picker.

Computer monitors are made
up of thousands of tiny squares
called pixels (if you look very
closely at your monitor you
should be able to see them).

![](img/colors.PNG)

When the screen is not turned
on, it's black because it's not
emitting any light. When it's
on, each pixel can be a different
color, creating a picture.

The color of every pixel on the
screen is expressed in terms of
a mix of red, green, and blue —
just like on a television screen.

![](img/colorpicker.PNG)

### Concepts 

![](img/rgb.PNG)

### Contrast 
When picking foreground and background
colors, it is important to ensure that there is
enough contrast for the text to be legible.

![](img/contract.PNG)

## CSS 3 

## Opacity 

CSS3 introduces the opacity
property which allows you to
specify the opacity of an element
and any of its child elements.
The value is a number between
0.0 and 1.0 (so a value of 0.5
is 50% opacity and 0.15 is 15%
opacity).

The CSS3 rgba property allows
you to specify a color, just like
you would with an RGB value,
but adds a fourth value to
indicate opacity. This value is
known as an alpha value and is
a number between 0.0 and 1.0
(so a value of 0.5 is 50% opacity
and 0.15 is 15% opacity). The
rgba value will only affect the
element on which it is applied
(not child elements).

```
p.one {
background-color: rgb(0,0,0);
opacity: 0.5;}
p.two {
background-color: rgb(0,0,0);
background-color: rgba(0,0,0,0.5);}
```
**Result**:
![](img/resutl.PNG)

### HSL Colors

CSS3 introduces an entirely new and intuitive
way to specify colors using hue, saturation,
and lightness values.

- hue 

Hue is the colloquial idea of
color. In HSL colors, hue is often
represented as a color circle
where the angle represents the
color, although it may also be
shown as a slider with values
from 0 to 360.

![](img/hue.PNG)

- saturation

Saturation is the amount of
gray in a color. Saturation is
represented as a percentage.
100% is full saturation and 0%
is a shade of gray

![](img/saturation.PNG)

### lightness 

Lightness is the amount of
white (lightness) or black
(darkness) in a color. Lightness
is represented as a percentage.
0% lightness is black, 100%
lightness is white, and 50%
lightness is normal. Lightness
is sometimes referred to as
luminosity.

![](img/lightness.PNG)

## Summury 


- Color not only brings your site to life, but also helps
convey the mood and evokes reactions.
- There are three ways to specify colors imn CSS :
RGB values, hex codes, and color names.

- Color picker can help you to find the color you want. 
- It is important to ensure that there is enough contrast between any text and the backgroung color.
- CSS3  has in troduced an extra value for RGB colors to indicate opacity. its is known as RGBA. 
- CSS3 also allows you to specify colors aas HSL values, 
with and optional opacity value. it is knon as HSLA.


## Text 

- There are properties to control the choice of font, size,
weight, style, and spacing.
- There is a limited choice of fonts that you can assume
most people will have installed.
- If you want to use a wider range of typefaces there are
several options, but you need to have the right license
to use them.
- You can control the space between lines of text,
individual letters, and words. Text can also be aligned
to the left, right, center, or justified. It can also be
indented.
- You can use pseudo-classes to change the style of an
element when a user hovers over or clicks on text, or
when they have visited a link.


## JPEG vs PNG vs GIF

### TL;DR

- Use JPEG format for all images that contain a natural scene or photograph where variation in colour and intensity is smooth.

- Use PNG format for any image that needs transparency or for images with text & objects with sharp contrast edges like logos.

- Use GIF format for images that contain animations.

### Comparison 

- **JPEG**

    lossy compression specification that takes advantage of human perception. It can achieve compression ratios of 1:10 without any perceivable difference in quality.

- **PNG** 

    is a lossless image format using DEFLATE compression. No data is lost during compression and no compression artefacts are introduced in the image.

- **GIF**

    a lossless image format that uses LZW compression algorithm. It was favoured over PNG for simple graphics in websites in its early days because the support of PNG was still growing.

### Transparency

In a simple form, transparency indicates something that is completely invisible. Logos and icons often need to be placed on backgrounds with variable colours. Hence it is desirable, that the background of these logos and icons is made transparent so that a single image can be used over multiple background variations.

- **JPEG**

    images don’t support transparency and are hence not usable for such cases.

- **PNG**

    images support transparency in two ways — inserting an alpha channel that allows partial transparency or by declaring a single colour as transparent (index transparency).

- **GIF**

    images support transparency by declaring a single colour in the colour palette as transparent (index transparency).


### Colours
There is a significant difference in the number of colours that can be supported by these 3 formats.

- **JPEG**

    images can support around 16 million colours. This is what makes them suitable for storing images of natural scenes.

- **PNG**

    images mainly have two modes — PNG8 and PNG24. PNG8 can support upto 256 colours whereas PNG24 can handle upto 16 million colours like a JPEG image.

- **GIF**

    images are limited to 256 colours. If index transparency is used, then one of these 256 colours is assigned as transparent and the remaining 255 are used for other colours.