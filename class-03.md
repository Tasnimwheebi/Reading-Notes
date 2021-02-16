# HTML Lists, CSS Boxes, JS Control Flow
## Lists
***
**Three different types of lists:**
* **Unordered lists** are lists that begin with a bullet point. it begin with a  `<ul>`.
* **Ordered lists** are lists where each item in the list is numbered `<ol>`.
 * **Definition lists** are made up of a set of terms along with the definitions for each of those terms 
    * `<dl>` : consists of a series of terms and
their definitions.
    * `<dt>` : This is used to contain the term being defined (the definition term).
    * `<dd>` : This is used to contain the definition.
 * **Nested list** : an `<li>` element to create a 
***
## Boxes 
## Boxes proporeties :
1. Border : The border separates the edge of one box from another.
2. Margin : Margins sit outside the edge of the border.
3. Padding : is the space between the border of a box and any content contained within it.
***

###  Box 
**width, height** dimensions: By default a box is sized just big
enough to hold its contents. To
set your own dimensions for a
box you can use the height and
width properties. By width and hight we can change its size.
* **LIMIT WIDTH** (min-width, max-width) .
the
min-width property specifies
the smallest size a box can be
displayed AND the
max-width property indicates
the maximum width a box can
stretch
* **Overflowing Content**: The overflow property tells the
browser what to do if the content
contained within a box is larger
than the box itself.
  - Hidden :This property simply hides any
extra content that does not fit in
the box.
  - scroll :This property adds a scrollbar to
the box so that users can scroll
to see the missing content.
### Border, Ma rgin & Padding : The padding and
margin properties are very helpful in adding space
between various items on the page.
* **BORDER** (border-width, border-color, border-style).
*  **PADDING** (padding-top,padding-right,padding-left, padding-bottom) 
*  **MARGIN** (margin-top,margin-right,margin-left,margin-bottom)
### GHANGING Inline/Block
  **text-align:left, right, center, top, bottom**
*  **Inline** :This causes a block-level element to act like an inline element
*  **block**: This causes an inline element to act like a block-level element.
*  **inline-block** :This causes a block-level element to flow like an inline element, while retaining other features of a block-level element.
*  **none** :this hidden an element .
### HIDING BOXES :The visibility property allows
you to hide boxes from users
but It leaves a space where the
element would have been.
*  hidden:This hides the element.
*  visible :This shows the element.
### Border Images:
The border-image property
applies an image to the border of
any box. It takes a background
image and slices it into nine
pieces.
### Box-shadow: 
The box-shadow property
allows you to add a drop shadow
around a box. It detirmined by :
 horizontal offset, vertical offeset, blur distance, spread of shadow
 ### Rounded Corners
The ability to
create rounded corners on any
box, using a property called
border-radius.
***
***
# **Basic JavaScript Instructions**
## **ARRAYS** :
**Is a special type of variable. It doesn't just store one value; it stores a list of values**  
*     var colors;

      colors = ['white', 'black', ' custom '];
 
## **VALUES IN ARRAYS** :
**Values in an array are accessed as if they are in a numbered list. It is important to know that the numbering of this list starts at zero (not one).**
   *     INDEX     VALUE
          0       'white'
          1       'black'
          2       'custom' 

## **ACCESSING & CHANGING VALUES IN AN ARRAY** :
*     // Create the array
      var colors = ['white', 
                    'black' ,
                    'custom']; 

      // Update the third item in the array  
      colors[2] = 'beige ' ;    

      // Get the element with an id of colors 
      var el = document .getElementByid(' colors') ;

      // Replace with third item from the array  
      el .textContent = colors[2]; 
             
***
***
***
# * Decisions and Loops**

## **SWITCH STATEMENTS**
A switch statement starts with a variable called the switch value. Each case indicates a possible value for this variable and the code that should run if the variable matches that value. 
## **IF ELSE VS IF SWITCH :**
| **IF ELSE** |  **SWITCH** |
| :---: | :---: | 
|There is no need to provide an else option. (You can just use an if statement.)With a series of if statements, they are all checked even if a match has been found (so it performs more slowly than switch).|   You have a default option that is run if none of the cases match. If a match is found, that code is run; then the break statement stops the rest of the switch statement running (providing better performance than multiple if statements). |

## **LOOPS :**
### Loops check a condition, If it returns true, a code block will run.Then the condition will be checked again and If it still return true, the code block will run again. It repeats until the condition return ## **FALSE** .
## **TYPE OF LOOPS :**
1. **FOR LOOP** : is often used to loop through the items in an array, also using for count numbers.
2. **WHILE LOOP** : usualy using for string count. 
3. **USI NG DO WHILE LOOPS** : The key difference between a whi1e loop and a do while loop is that the statements in the code block come before the condition. This means that those statements are run once whether or not the condition is met. 
***
## **KEY LOOP CONCEPTS :**
* KEYWORDS
1. **break** This keyword causes the termination of the loop and tells the interpreter to go onto the next statement of code outside of the loop. (You may also see it used in functions.) 
2. **continue** This keyword tells the interpreter to continue with the current iteration, and then check the condition again. (If it is true, the code runs again.) 
* 

