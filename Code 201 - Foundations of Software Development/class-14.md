# CSS Transforms, Transitions, and Animations

- The Fade in is great way to emphasize functionality or draw attention to a call to action. (Make sure you set the class of your div to “fade” to see this working.)

- To grow an element, you used to have to use its width and height, or its padding. But now we can use CSS3’s transform to enlarge. (Set your div’s class to “grow” and then add this code to your style block)

- CSS transforms have a number of different uses, and one of the best is transforming the rotation of an element.

- A really popular effect at the moment is transitioning a square element into a round one, and vice versa. With CSS, it’s a simple effect to achieve, we just transition the border-radius property.

- 3D shadows were frowned upon for a year or so, because they weren’t seen as compatible with flat design, which is of course nonsense, they work fantastically well to give a user feedback on their interactions and work with flat, or fake 3D interfaces. (This effect is achieved by adding a box shadow, and then moving the element on the x axis using the transform and translate properties so that it appears to grow out of the screen.)

- Not all elements use the transition property. We can also create highly complex animations using @keyframes, animation and animation-iteration.
- In this case, we’ll first define a CSS animation in your styles. You’ll notice that due to implementation issues, we need to use @-webkit-keyframes as well as @keyframes (yes, Internet Explorer really is better than Chrome, in this respect at least).

```
The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values. As mentioned, for a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes. There are four transition related properties in total, including transition-property, transition-duration, transition-timing-function, and transition-delay. Not all of these are required to build a transition, with the first three are the most popular.
```
