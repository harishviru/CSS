                                 CSS Position and Z-index

CSS Position
------------
.The position property specifies the type of positioning method used for an element 
(static, relative, fixed, absolute or sticky).

There are five different position values:

i)static         (Default)
ii)relative
iii)fixed
iv)absolute
v)sticky

i)i)position: static;
.Static positioned elements are not affected by the top, bottom, left, and right properties.
.An element with position: static; is not positioned in any special way; 
 it is always positioned according to the normal flow of the page.

 ii)relative
.An element with position: relative; is positioned relative to its normal position.
.Setting the top, right, bottom, and left properties of a relatively-positioned element
 will cause it to be adjusted away from its normal position.

 
iii)fixed
.An element with position: fixed; is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled. 
The top, right, bottom, and left properties are used to position the element.

iv)absolute
.An element with position: absolute; is positioned relative to the nearest positioned ancestor .
.However; if an absolute positioned element has no positioned ancestors, 
 it uses the document body, and moves along with page scrolling.

Note: A "positioned" element is one whose position is anything except static.

v)sticky
.An element with position: sticky; is positioned based on the user's scroll position.
A sticky element toggles between relative and fixed, depending on the scroll position.

 short cuts info :
 i)static               :default position of any html element
 ii)relative            :this is positioned relative to its own
 iii)absolute           :this is positioned relative to its parent
 iv)fixed               :this is a fixed element in the given position    
 v)sticky               :this is to sticky any element in the given position



Z-index :
--------
i)z-index:      auto|number|initial|inherit;                [DefVal :auto]

.The z-index property specifies the stack order of an element.
.An element with greater stack order is always in front of an element with a lower stack order.

Note: z-index ONLY works on positioned elements (position: absolute, position: relative, position: fixed, or position: sticky).

ex :
  position: absolute;
  left: 0px;
  top: 0px;
  z-index: -1;
















