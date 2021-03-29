
#  jQuery, Events, and The DOM
* **Events are the browser's way of indicating when
something has happened (such as when a page has
finished loading or a button has been clicked).**
* **Binding is the process of stating which event you are
waiting to happen, and which element you are waiting
for that event to happen upon.**
* **When an event occurs on an element, it can trigger a
JavaScript function. When this function then changes
the web page in some way, it feels interactive because
it has responded to the user.**
* **You can use event delegation to monitor for events
that happen on all of the children of an element.**
* **The most commonly used events are W3C DOM
events, although there are others in the HTMLS
specification as well as browser-specific events.**

# what is jQuery ?
It is just a JavaScript file but estimates show it has been used on over a
quarter of the sites on the web, because it makes coding simpler.

jQuery's motto is "Write less, do more," because it allows you to achieve
the same goals but in fewer lines of code than you would need to write
with plain JavaScript.

## FINDING ELEMENTS
The • htm 1 () and • text () methods both retrieve and update the content
of elements. This page will focus on how to retrieve element content.
* html() :
When this method is used to retrieve information
from a jQuery selection, it retrieves only the HTML
inside the first element in the matched set, along
with any of its descendants.
* text() :
When this method is used to retrieve the text from
a jQuery selection, it returns the content from every
element in the jQuery selection, along with the text
from any descendants.

## UPDATING ELEMENTS

Here are four methods that update the content
of all elements in a jQuery selection .
* html() 
* text()
* replaceWith() 
* remove()

## INSERTING ELEMENTS 
Inserting new elements involves two steps:
1. Create the new elements in a jQuery object
2. Use a method to insert the content into the page:
* before()
* after()
* prepend()
* prepend()

## GETTING AND SETTING ATTRIBUTE VALUES

You can create attributes, or access and update
their contents, using the following four methods.

* attr()
* removeAttr()
* addCl ass()
* removeClass()
