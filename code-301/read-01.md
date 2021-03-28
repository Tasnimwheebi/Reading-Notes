# SMACSS and Responsive Web Design
## RESPONSIVE WEB DESIGN and FLOATS
### RESPONSIVE WEB DESIGN :
**Is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop.**
### Responsive vs. Adaptive vs. Mobile
* Responsive generally means to react quickly and positively to any change.
* Adaptive means to be easily modified for a new purpose or situation, such as change.
* Mobile generally means to build a separate website commonly on a new domain solely for mobile users.


### Responsive web design is broken down into three main components :
* Flexible Layouts :
is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width.
* Media Queries :Media queries were built as an extension to media types commonly found when targeting and including styles. Media queries provide the ability to specify different styles for individual browser and device circumstances, the width of the viewport or device orientation for example.
    * Initializing Media Queries:

    There are a couple different ways to use media queries, using the @media rule inside of an existing style sheet, importing a new style sheet using the @import rule, or by linking to a separate style sheet from within the HTML document.
    * Logical Operators in Media Queries:

    Logical operators in media queries help build powerful expressions. There are three different logical operators available for use within media queries, including and, not, and only.
    * Media Features in Media Queries:
    Media features identify what attributes or properties will be targeted within the media query expression.

    1. Height & Width Media Features
    2. Orientation Media Feature
    3. Aspect Ratio Media Features
    4. Resolution Media Feature

    * Media Queries Demo
* Flexible Media


# What is “Float”?
There are four valid values for the float property. Left and Right float elements those directions respectively. None (the default) ensures the element will not float and Inherit which will assume the float value from that elements parent element.

## Clearing the Float
Clear has four valid values as well. Both is most commonly used, which clears floats coming from either direction. Left and Right can be used to only clear the float from one direction respectively. None is the default, which is typically unnecessary unless removing a clear value from a cascade. Inherit would be the fifth, but is strangely not supported in Internet Explorer. Clearing only the left or right float, while less commonly seen in the wild, definitely has its uses.

