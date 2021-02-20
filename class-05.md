# **HTML Images; CSS Color & Text**
## **IMEGES**
### **`<img>`**
### The `<img>` element is used to add images to a web page.
Exaple to add an image : `<img src="images/flower.jpg" alt="flower image"`
* **src** :
This tells the browser where
it can find the image file.
* **alt** :
This provides a text description
of the image which describes the
image if you cannot see it.
* **title** :
You can also use the title
attribute with the <img> element
to provide additional information
about the image. For example : `<img scr=" " alt=" ">`title="you can add here information about the flower".
### **Height & Width of Images.**
You will also often see an <img>
element use two other attributes
that specify its size:
* **Height** :
This specifies the height of the
image in pixels.`<img src="pwth.jpg" alt="name of the img" height="450" />`
* **Width** :
This specifies the width of the
image in pixels. `<img src="pwth.jpg" alt="name of the img" width="450" />`
### **IMAGE PLACEMENT**
Here are three
examples of image placement
that produce different results:
* Before a paragraph:
The paragraph starts on a new
line after the image.`<img src="pwth.jpg" alt="name of the img" />` 
`<P> </P>`.
* Inside the start of a
paragraph :
The first row of text aligns with
the bottom of the image.`<P>`  `<img src="pwth.jpg" alt="name of the img"/>` ......... `</P>`
* in the middle of a
paragraph
The image is placed between the
words of the paragraph that it
appears in. `<P>` ............... `<img src="pwth.jpg" alt="name of the img"/>` ......... `</P>`.


Where you place the image in
the code is important because
browsers show HTML elements
in one of two ways:
* Block elements always appear
on a new line. Examples of block
elements include the `<h1>` and
`<p>` elements.
If the `<img>` is followed by a
block level element (such as a
paragraph) then the block level
element will sit on a new line.
* Inline elements sit within a
block level element and do not
start on a new line. Examples of
inline elements include the `<b>`,
`<em>`, and `<img>` elements.
If the `<img>` element is inside a
block level element, any text or
other inline elements will flow
around the image.

**ALIGN** 

The align attribute was
commonly used to indicate how
the other parts of a page should
flow around an image.

**The align attribute can take
these horizontal values:**
* **left** : 
This aligns the image to the left
(allowing text to flow around its
right-hand side).`<P>` ............... `<img src="pwth.jpg" alt="name of the img"align="left"/>` ......... `</P>`.

* **right**
This aligns the image to the right
(allowing text to flow around its
left-hand side). `<P>` ............... `<img src="pwth.jpg" alt="name of the img"align="right"/>` ......... `</P>`.

There are three values that the
align attribute can take that
control how the image should
align vertically with the text that
surrounds it:
* **TOP**
This aligns the first line of the
surrounding text with the top of
the image.`<P>` ............... `<img src="pwth.jpg" alt="name of the img"align="top"/>` ......... `</P>`.
* **MIDDLE**
This aligns the first line of the
surrounding text with the middle
of the image.`<P>` ............... `<img src="pwth.jpg" alt="name of the img"align="middle"/>` ......... `</P>`.
* **BOTTOM**
This aligns the first line of the
surrounding text with the bottom
of the image.`<P>` ............... `<img src="pwth.jpg" alt="name of the img"align="bottom"/>` ......... `</P>`.
### Three Rules for Creating Images
1. Save images in the right format.
2. Save images at
the right size.
3. Use the correct
resolution.

