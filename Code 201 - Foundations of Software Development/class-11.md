# Images

Controlling the size and alignment of
your images using CSS keeps rules that
affect the presentation of your page in
the CSS and out of the HTML markup.

## Controlling sizes of images in css

You can control the size of an
image using the width and
height properties in CSS, just
like you can for any other box.

Specifying image sizes helps
pages to load more smoothly
because the HTML and CSS
code will often load before the
images, and telling the browser
how much space to leave for an
image allows it to render the rest
of the page without waiting for
the image to download.

## aligning images using css

In the last chapter, you saw how
the float property can be used
to move an element to the left or
the right of its containing block,
allowing text to flow around it.

Rather than using the `<img>`
element's align attribute, web
page authors are increasingly
using the float property to align
images. There are two ways that
this is commonly achieved:

1: The float property is added
to the class that was created to
represent the size of the image
(such as the small class in our
example)

2: New classes are created with
names such as align-left or
align-right to align the images
to the left or right of the page.
These class names are used in
addition to classes that indicate
the size of the image.

## Background images

`background-image`

The background-image
property allows you to place
an image behind any HTML
element. This could be the entire
page or just part of the page. By
default, a background image will
repeat to fill the entire box.

The path to the image follows
the letters url, and it is put
inside parentheses and quotes.

## Repeating images

`background-repeat`
`background-attachment`

the background property can have four values.

- `repeat`

  The background image is
  repeated both horizontally and
  vertically (the default way it
  is shown if the backgroundrepeat property isn't used).

- `no-repeat`

  The background-attachment
  property specifies whether a
  background image should stay in
  one position or move as the user
  scrolls up and down the page.

- Background Position

`background-position`

When an image is not being
repeated, you can use the
background-position
property to specify where in the
browser window the background
image should be placed.

This property usually has a pair
of values. The first represents
the horizontal position and the
second represents the vertical.

## Summary

- You can specify the dimensions of images using CSS.
  This is very helpful when you use the same sized
  images on several pages of your site.
- Images can be aligned both horizontally and vertically
  using CSS.
- You can use a background image behind the box
  created by any element on a page.
- Background images can appear just once or be
  repeated across the background of the box.
- You can create image rollover effects by moving the
  background position of an image.
- To reduce the number of images your browser has to
  load, you can create image sprites.

# Practical inforamtion

To wrap up the book we are going to look
at some practical information that will
help you launch a successful site.

## Search Engine Optimization (SEO)

SEO is a huge topic and several books have been written on the subject.
The following pages will help you understand the key concepts so you can
improve your website's visibility on search engines.

## How Many People Are Coming to Your Site?

The overview page gives you a snapshot of the key information you are
likely to want to know. In particular, it tells you how many people are
coming to your site.

## Summary

- Search engine optimization helps visitors find your
  sites when using search engines.
- Analytics tools such as Google Analytics allow you to
  see how many people visit your site, how they find it,
  and what they do when they get there.
- To put your site on the web, you will need to obtain a
  domain name and web hosting.
- FTP programs allow you to transfer files from your
  local computer to your web server.
- Many companies provide platforms for blogging, email
  newsletters, e-commerce and other popular website
  tools (to save you writing them from scratch).

# HTML 5 Video and audio

The `<video>` and `<audio>` elements allow us to embed video and audio into web pages. As we showed in Video and audio content, a typical implementation looks like this:

```
<video controls>
  <source src="rabbit320.mp4" type="video/mp4">
  <source src="rabbit320.webm" type="video/webm">
  <p>Your browser doesn't support HTML5 video. Here is a <a href="rabbit320.mp4">link to the video</a> instead.</p>
</video>
```

## The HTMLMediaElement API

Part of the HTML5 spec, the **HTMLMediaElement API** provides features to allow you to control video and audio players programmatically — for example HTMLMediaElement.play().

## Summary

I think we've taught you enough in this article. The **HTMLMediaElement API** makes a wealth of functionality available for creating simple video and audio players, and that's only the tip of the iceberg. See the "See also" section below for links to more complex and interesting functionality.

1. The time display currently breaks if the video is an hour long or more (well, it won't display hours; just minutes and seconds). Can you figure out how to change the example to make it display hours?

1. Because `<audio>` elements have the same HTMLMediaElement functionality available to them, you could easily get this player to work for an `<audio>` element too. Try doing so.

1. Can you work out a way to turn the timer inner `<div>` element into a true seek bar/scrobbler — i.e., when you click somewhere on the bar, it jumps to that relative position in the video playback? As a hint, you can find out the X and Y values of the element's left/right and top/bottom sides via the getBoundingClientRect() method, and you can find the coordinates of a mouse click via the event object of the click event, called on the Document object. For example:

```
document.onclick = function(e) {
  console.log(e.x) + ',' + console.log(e.y)
}
```
