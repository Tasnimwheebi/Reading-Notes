# Responsive Web Design and Regular Expressions
##  CSS GRID
CSS Grid Layout (aka “Grid”), is a two-dimensional grid-based layout system that aims to do nothing less than completely change the way we design grid-based user interfaces.

### **Grid properties**
Grid :
A shorthand for setting all of the following properties in a single declaration: grid-template-rows, grid-template-columns, grid-template-areas, grid-auto-rows, grid-auto-columns, and grid-auto-flow 
### Properties for the Parent
Grid Container
* display : 
Defines the element as a grid container and establishes a new grid formatting context for its contents.
* grid-template-columns ,
grid-template-rows :
Defines the columns and rows of the grid with a space-separated list of values. The values represent the track size, and the space between them represents the grid line.
The fr unit allows you to set the size of a track as a fraction of the free space of the grid container.
* grid-template-areas :
Defines a grid template by referencing the names of the grid areas which are specified with the grid-area property. Repeating the name of a grid area causes the content to span those cells. A period signifies an empty cell. The syntax itself provides a visualization of the structure of the grid.
* grid-template:
A shorthand for setting grid-template-rows, grid-template-columns, and grid-template-areas in a single declaration.
* column-gap ,
row-gap ,
grid-column-gap ,
grid-row-gap:
Specifies the size of the grid lines. You can think of it like setting the width of the gutters between the columns/rows.
* gap ,
grid-gap:A shorthand for row-gap and column-gap.
* justify-items : Aligns grid items along the inline (row) axis (as opposed to align-items which aligns along the block (column) axis). 
* align-items :
Aligns grid items along the block (column) axis (as opposed to justify-items which aligns along the inline (row) axis).
* place-items :place-items sets both the align-items and justify-items properties in a single declaration.
* justify-content : Sometimes the total size of your grid might be less than the size of its grid container. This could happen if all of your grid items are sized with non-flexible units like px. In this case you can set the alignment of the grid within the grid container. This property aligns the grid along the inline (row) axis (as opposed to align-content which aligns the grid along the block (column) axis).
* align-content :Sometimes the total size of your grid might be less than the size of its grid container. This could happen if all of your grid items are sized with non-flexible units like px. In this case you can set the alignment of the grid within the grid container. This property aligns the grid along the block (column) axis (as opposed to justify-content which aligns the grid along the inline (row) axis).
* place-content:
place-content sets both the align-content and justify-content properties in a single declaration.
* grid-auto-columns ,
grid-auto-rows:
Specifies the size of any auto-generated grid tracks (aka implicit grid tracks). Implicit tracks get created when there are more grid items than cells in the grid or when a grid item is placed outside of the explicit grid.
* grid-auto-flow :
If you have grid items that you don’t explicitly place on the grid, the auto-placement algorithm kicks in to automatically place the items. This property controls how the auto-placement algorithm works.
