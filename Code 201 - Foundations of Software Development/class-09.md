# Html-Forms

Traditionally, the term 'form' has referred
to a printed document that contains
spaces for you to fill in information.

## How forms works 

A user fills in a form and then presses a button
to submit the information to the server.

![](img/forms-structure.PNG)

A form may have several form controls, each
gathering different information. The server
needs to know which piece of inputted data
corresponds with which form element.

![](img/formname.PNG)

## Summary for forms

- Whenever you want to collect information from
visitors you will need a form, which lives inside a
`<form>` element.
- Information from a form is sent in name/value pairs.
- Each form control is given a name, and the text the
user types in or the values of the options they select
are sent to the server.
- HTML5 introduces new form elements which make it
easier for visitors to fill in forms.


# Lists, Tables and Forms

There are several CSS properties that
were created to work with specific types
of HTML elements, such as lists, tables,
and forms.

-  In addition to the CSS properties covered in other
chapters which work with the contents of all elements,
there are several others that are specifically used to
control the appearance of lists, tables, and forms.
-  List markers can be given different appearances
using the list-style-type and list-style image
properties.
-  Table cells can have different borders and spacing in
different browsers, but there are properties you can
use to control them and make them more consistent.
-  Forms are easier to use if the form controls are
vertically aligned using CSS.
-  Forms benefit from styles that make them feel more
interactive.

# JS Events

When you browse the web, your browser registers different
types of events. It's the browser's way of saying, "Hey, this
just happened." Your script can then respond to these events. 


## Event Flow

Html Elements nest inside other elements, if you hover or click on a link, you will also be hovring or clicking on it's parent element. 

- Event handlers/ listners can be bound to the containing html elements plus document object and window object. the order in which events fire is know as event flow, and events flow in two directions.

## Why flow matters 

The flow of events only really matters when you code has events handlers on an element and one of it's ancestor or descendeant elements.

### The event Object 

When events occurs, the event object tells you information about the event, and the element it happend upon.

### Event Listner with no parameters 
![](img/event listner.PNG)

### Event Listner with parametrs 

![](img/elwparams.PNG)

### Changing default behavior

The event object has methods that change:
the default behavior of an element and how
the element's ancestors respond to the event. 

## MOUSE EVENTS

The mouse events are fired when the mouse is moved and also when its
buttons are clicked. 

- CLICK:

    The aim of this example is to use
    the c 1 i ck event to remove the
    big note that has been added to
    the middle of the page. But first,
    the script has to create that note.

    ```
    II Create the HTML for the message
CLICK
When the c 1 i ck event fires on
the close link the di smi ssNote()
function is called. This function
will remove the note that was
added by the same script.
```
var msg = '<div class=\"header\"><a id=\"close\" href=" #">close X</a><ldiv>';
msg += '<div><h2>System Maintenance</h2>';
msg += 'Our servers are being updated between 3 and 4 a.m. ' ;
msg += 'Duri ng this t ime, there may be minor disrupti ons to service.</div>' ;
var elNote = document.createElement( 'div');
elNote.setAttribute( 'i d' , 'note');
elNote . innerHTML = msg;
document.body.appendChi l d{elNote);
function dismissNote() {
document.body. removeChi l d{elNote);
// Create a new el emen t
//Add an id of note
//Add the message
II Add it to the page
// Declare functi on
II Remove the note
var elClose = document.getElementByid('close '); // Get the close button
elClose .addEventl istener( ' click', dismissNote, false);// Cl ick cl ose-clear note
``` 
### Where events occur

the event object tell you where the cursor was positioned when an event was triggered.



    

