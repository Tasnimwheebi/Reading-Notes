#
## Form Controls:
There are several types of form controls that
you can use to collect information from visitors
to your site.
* **ADDING TEXT**: 
    * Text input (single-line)
    * Password input
    * Text area (multi-line)
* **Making Choices:**
    * Radio buttons
    * Checkboxes
    * Drop-down boxes
* **Submitting Forms:**
    * Submit buttons
    * Image buttons
* **Uploading Files:**
    * File upload

### How Forms Work :
1. A user fills in a form and then presses a button
to submit the information to the server.
2. The name of each form
control is sent to the
server along with the
value the user enters or
selects.
3. The server processes
the information using a
programming language
such as PHP, C#, VB.net,
or Java. It may also store
the information in a
database.
2. The server creates a new
page to send back to the
browser based on the
information received.

## Form Structure
* Form controls live inside a
`<form>` element. This element
should always carry the action
attribute and will usually have a
method and id attribute too.
* Every `<form>` element requires
an action attribute.
* method
Forms can be sent using one of
two methods: get or post.
    * The get
method is ideal for: 
        1. short forms (such as search
boxes)
        2.  when you are just retrieving
data from the web server
(not sending information that
should be added to or deleted
from a database)

    * you should use the
post method if your form:
        1. allows users to upload a file
        2.  is very long
        3. contains sensitive data
(e.g. passwords)
        4. adds information to, or
deletes information from, a
database.
* id .


