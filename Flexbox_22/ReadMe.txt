    
                      Flexible Box Module
                      ===================  
    .CSS Flexible Box Module -one dimensionl layout model.
    .flexible and efficient layouts
    .distribute space among items
    .control their alignment.

 Before flex box ,there are four layout modes.
 .Block ,for section in a webpage
 .lnline,for text
 .Table,for two-dimensional table data
 .positioned,for explicit position of an element     
Note :But these layout modes does not provide flexiblilty   


With Flex box :(Why flex box )
.a lot of flexibility
.arrange items
.spacing
.alignment
.order of items
.bootsrap 4 built on top of the flex layout.

Terminology :

 <div class="flex-container">
  <div>1</div>
  <div>2</div>
  <div>3</div>
</div> 

 we have two items as 
    i)Parent or flex-container
   ii)Children or flex-items


we have flex-axis,they are 
 i)Main Axis   (Horizantal)
ii)Cross Axis  (Vertical)
                        ____________________________  cross start
                      |                         |     |     |
                      |  item1 item2.....etc    |     |Cross size   
                      |______________________|__|___cross end
                      |                                       |
                      |---------Main size ------------ -------|
           Main start                                       Main end      

Flex Container properties :
----------------------------
i)display                                :flex,inline-flex.
ii)flex-direction                        :column ,column-reverse,row, row-reverse  
iii)flex-wrap                            :wrap,nowrap,wrap-reverse.    
iv)flex-flow
v)justify-content                         :center,flex-start,flex-end,space-evenly,space-around,space-between.
vi)align-items                            : 
vii)align-content



flex-direction      :column ,column-reverse,row, row-reverse           [defVal:row]
 .The flex-direction property defines in which direction the container wants to stack the flex items.

 flex-wrap         :wrap,nowrap,wrap-reverse.                          [defval:nowrap]      
.The flex-wrap property specifies whether the flex items should wrap or not.

flex-flow      (Short hand property)
The flex-flow property is a shorthand property for setting both the flex-direction and flex-wrap properties.
 flex-flow : flex-direction flex-wrap; 
 ex : flex-flow: row nowrap;


justify-content   :center,flex-start,flex-end,space-evenly,space-around,space-between (Horizontaly)    [DefVal:flex-start]
The justify-content property is used to align the flex items:
ex :  justify-content: center;

align-items        :center,flex-start,flex-end,stretch,baseline          [defVal:stretch]        (Vertically)
The align-items property is used to align the flex items.
ex :align-items :stretch.

align-content  : center,flex-start,flex-end,stretch,space-around,space-between   [defVal:stretch]       (vertically)                               
The align-content property is used to align the flex lines.

Flex item or children properties:
----------------------------------------------
i)order
ii)flex-grow
iii)flex-shrink
iv)flex-basis
v)flex
vi)align-self

order             :    number      [defVal:0]
The order property specifies the order of the flex items.


flex-grow    : number          [defVal:0]
The flex-grow property specifies how much a flex item will grow relative to the rest of the flex items.


flex-shrink   : number          [defVal:1]
The flex-shrink property specifies how much a flex item will shrink relative to the rest of the flex items.


flex-basis  :number           [defVal:auto]                                                           
The flex-basis property specifies the initial length of a flex item.  (It acts like width,instead of width we can use these)


flex             :short hand property 
The flex property is a shorthand property for the flex-grow, flex-shrink, and flex-basis properties.
     flex :flex-grow flex-shrink flex-basis;
ex : flex :0 1 auto;







