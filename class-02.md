# HTML Text, CSS Introduction, and Basic JavaScript Instructions
## TEXT 
The tags in html provide us extra meaning
and allow browsers to show users the
appropriate structure for the page.
## Structural markup:
 The elements that you can use to
describe both headings and paragraphs
## Semantic markup:
which provides us extra information.

# HTML TAGS :
### HEADING : 
HTML has six "levels" of headings: h1 , h2, h3, h4, h5, h6.
Browsers display the contents of
headings at different sizes. The contents of an h1  element is the largest, and the contents of an h6  element is the smallest.
### PARAGRAPH
By default, a browser will show each paragraph on a new line with some space between it and any subsequent paragraphs.
### BOLD & ITALIC 
* BOLD : By enclosing words in the tags
< b > and < /b > we can make
characters appear bold.
* ITALIC :By enclosing words in the tags
< i > and </ i > we can make
characters appear italic.
### Superscript & Subscrip
* The superscript < sup > element is used
to contain characters that should be superscript such
as the suffixes of dates or mathematical concepts ike
raising a number to a power .
* The subscrip < sub > element is used to
contain characters that should be subscript. It is commonly used with foot notes or chemical formulas such as H20.
### White Space
When the browser comes across
two or more spaces next to each
other, it only displays one space.
Similarly if it comes across a line
break, it treats that as a single
space too. This is known as
white space collapsing.
## Line Breaks & Horizontal Rules 
* **< br />** the browser will automatically show each new paragraph or heading on a new line.
* **< hr />**  you can add a horizontal rule between sections using the < hr /> tag.
## Visual Editors & Their Code views
Content management systems and HTML editors have two views of the page you are creating: a visual editor and a code view.

## Semantic Markup
There are some text elements that are not intended to affect the
structure of your web pages, but they do add extra information to the
pages — they are known as semantic markup.  For example,
the content of the < em >
element is shown in italics,
the < blockquote >
element which indicates that a
block of text is a quotation.
### Strong & Emphasis
* The use of the < strong >
element indicates that its
content has strong importance
* The content of the < em >
element is shown in italics.
### QOUTATION
There are two elements
commonly used for marking up
quotations:
* The < blockquote> element is
used for longer quotes.
* The < q> element is used for
shorter quotes
### Abbreviations & Acronyms
If you use an abbreviation or
an acronym, then the < abbr >
element can be used. A title
attribute on the opening tag is
used to specify the full term.
### Citations & Definitions
 * The < cite > element can be used to indicate where the citation is from.
 * The < dfn > element is used to indicate the defining instance of a new term.
 ### Author Details
 The < address > element has
quite a specific use: to contain
contact details for the author of
the page.
### Changes to Content
* The < ins > element can be used
to show content that has been
inserted into a document, while
the < del > element can show text
that has been deleted from it.
* The < s> element indicates
something that is no longer
accurate or relevant.

# Introducing CSS

## BLOCK & INLINE ELEMENTS
* BLOCK  level elements look
like they start on a new line. 
* INLINE elements flow within the
text and do not start on a new
line.


CSS works by associating rules with HTML elements. These rules govern
how the content of specified elements should be displayed. A CSS rule
contains two parts: a selector and a declaration.

CSS declarations sit inside curly brackets and each is made up of two
parts: a property and a value, separated by a colon. You can specify
several properties in one declaration, each separated by a semi-colon
## THREE WAYS TO STYLE THE HTML PAGE BY CSS:

### Using External CSS
 The < link > element can be used
in an HTML document to tell the
browser where to find the CSS
file used to style the page.
### Using Internal CSS
You can also include CSS rules
within an HTML page by placing
them inside a < style > element,
which usually sits inside the
< head > element of the page.
### CSS Selectors
1. Universal Selector
1. Type Selector
2. Class Selector
2. ID Selector
3. Child Selector
2. Descendant Selector
3. Adjacent Sibling Selector
3. General Sibling
Selector

# Basic JavaScript Instructions
## STATEMENTS 
A script is a series of instructions that a computer can follow one-by-one.
Each individual instruction or step is known as a statement.
## COMMENTS
You should write comments to explain what your code does.
They help make your code easier to read and understand.
This can help you and others who read your code. 
## VARIABLE
A script will have to temporarily
store the bits of information it
needs to do its job. It can store this
data in variables.
## DATA TYPES 
1. NUMERIC DATA TYPE 
2. STRING DATA TYPE 
3. BOOLEAN DATA TYPE 
## ARRAYS
An array is a special type of variable. It doesn't
just store one value; it stores a list of values. 
### VALU ES IN ARRAYS
Values in an array are accessed as if they are in
a numbered list. It is important to know that the
numbering of this list starts at zero (not one). 
## EXPRESSIONS
An expression evaluates into (results in) a single value. Broadly speaking
there are two types of expressions. 
1. EXPRESSIONS THAT JUST ASSIGN A
VALUE TO A VARIABLE 
2. EXPRESSIONS THAT USE TWO OR
MORE VALUES TO RETURN A
SINGLE VALUE 
## OPERATORS
Expressions rely on things called operators; they allow programmers to
create a single value from one or more values. 
1. ASSIGNMENT OPERATORS
2. COMPARISON OPERATORS 
3. ARITHMETIC OPERATORS
4. LOGICAL OPERATORS
1. STRING OPERATORS
## SWITCH STATEMENTS
A switch statement starts with a
variable called the switch value.
Each case indicates a possible
value for this variable and the
code that should run if the
variable matches that value. 
