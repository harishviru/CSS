                                 Grid
                                 ----
 The CSS Grid Layout Module offers a grid-based layout system, with rows and columns, 
 making it easier to design web pages without having to use floats and positioning.  

 .An HTML element becomes a grid container when its display property is set to grid or inline-grid.

.grid-container {
  display: grid|inline-grid;
}

.All direct children of the grid container(Parent) automatically become grid items.
.The vertical lines of grid items are called columns.
.The horizontal lines of grid items are called rows.
The spaces between each column/row are called gaps.

Parent grid properties :
i)display                                          :grid|inline-grid;
ii)grid-auto-flow                                  :row, column, or dense.   [defVal:row]
iii)grid-template-rows                             :
iv)grid-template-columns                           :auto auto auto auto ...etc

v) grid-column-gap                                 :
vi)grid-row-gap                                    :
vii)grid-gap                                       :

viii)grid-template-areas                           :
ix) justify-content (horizontally)                 :start|end|center|space-evenly|space-around|space-between.
x)align-content   (vertically)                     : start|end|center|space-evenly|space-around|space-between.                           
xi)grid-auto-rows           
xii)grid-auto-columns
Note : The grid-template-columns property overrides grid-auto-columns property.


 grid-template-columns :
.The grid-template-columns property defines the number of columns in your grid layout, and it can define the width of each column.
 grid-template-columns                              :auto auto auto auto;

grid-template-rows
.The grid-template-rows property defines the height of each row.
 grid-template-rows: 80px 200px;

grid-column-gap
.The grid-column-gap property sets the gap between the columns:
 grid-column-gap: 50px;

grid-row-gap
.The grid-row-gap property sets the gap between the rows
  grid-column-row: 50px;

  grid-gap
.The grid-gap property is a shorthand property for the grid-row-gap and the grid-column-gap properties:
 grid-gap  :grid-row-gap grid-column-gap ;

  justify-content (horizontally):start|end|center|space-evenly|space-around|space-between.
 .The justify-content property is used to align the whole grid inside the container.

align-content   (vertically)      : start|end|center|space-evenly|space-around|space-between.                           
.The align-content property is used to vertically align the whole grid inside the container.


Child grid properties :
i)grid-row                      :grid-row-start grid-row-end   ( ex :2/4)
ii)grid-row-start
iii)grid-row-end
.The grid-row property defines on which row to place an item.
Note: The grid-row property is a shorthand property for the grid-row-start and the grid-row-end properties.

iv)grid-column           : grid-column-start grid-column-end  ( ex :2/4)
v)grid-column-start
vi)grid-column-end
.The grid-column property defines on which column(s) to place an item.
Note: The grid-column property is a shorthand property for the grid-column-start and the grid-column-end properties.

(grid-area  short hand property for grid-row-start,grid-column-start,grid-row-end and grid-column-end.)
vii)grid-area :grid-row-start,
                       grid-column-start,
                      grid-row-end,
                      grid-column-end . 

Naming Grid Items :
----------------------------
In child item , we have to give  like
         grid-area: myArea;

In Parent Container ,we have to give like
         grid-template-areas: 'myArea myArea myArea myArea myArea';
           or 
       grid-template-areas: 'myArea myArea myArea myArea  .';
         

.repeat()
grid-template-rows :10px 10px 10px;
      =
 grid-template-rows :repeat(3,10px);  
   =
 grid-template-rows :10px repeat(2,10px);  




























