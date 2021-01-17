 i)resize                 : none|both|horizontal|vertical|initial|inherit;                             [defVal:none]
The resize property defines if (and how) an element is resizable by the user.

The resize property does not apply to inline elements or to block elements where overflow="visible". 
So, make sure that overflow is set to "scroll", "auto", or "hidden".    

ii)var() 
The var() function is used to insert the value of a CSS variable.
Syntax:var(name, value)

name 	Required. The variable name (must start with two dashes)
value 	Optional. The fallback value (used if the variable is not found)
ex :
:root {
  --main-bg-color: coral;
  --main-txt-color: blue;
  --main-padding: 15px;
}

#div1 {
  background-color: var(--main-bg-color);
  color: var(--main-txt-color);
  padding: var(--main-padding);
}

#div2 {
  background-color: var(--main-bg-color);
  color: var(--main-txt-color);
  padding: var(--main-padding);
}

iii)calc()
The calc() function performs a calculation to be used as the property value.
 syntax : calc(expression)
 ex :
 #div1 {
  position: absolute;
  left: 50px;
  width: calc(100% - 100px);
  border: 1px solid black;
}

iv)attr()
 The attr() function returns the value of an attribute of the selected elements.
 syntax : attr(attribute-name)

ex :
a:after {
  content: " (" attr(href) ")";
}


|Gradient Backgrounds|
=====================
.CSS gradients let you display smooth transitions between two or more specified colors.

CSS defines two types of gradients:

.Linear Gradients (goes down/up/left/right/diagonally)
.Radial Gradients (defined by their center)

a)CSS Linear Gradients  : Top to Bottom (this is default)

.To create a linear gradient you must define at least two color stops. 
Color stops are the colors you want to render smooth transitions among.
You can also set a starting point and a direction (or an angle) along with the gradient effect.

syntax :
background-image: linear-gradient(direction, color-stop1, color-stop2, ...);

ex :background-image: linear-gradient(red, yellow);  //Top to Bottom (this is default)

    background-image:linear-gradient(to right ,red,yellow);//left to right
      //Direction - Diagonal
    background-image:liner-gradient(to bottom right,red,yellow);//top left to bottom right

    background-image:liner-gradient(to bottom left,red,yellow);//top right to bottom left

Using Angles
---------------
.If you want more control over the direction of the gradient, you can define an angle,
 instead of the predefined directions (to bottom, to top, to right, to left, to bottom right, etc.). 
  i)A value of 0deg is equivalent to "to top". 
  ii)A value of 90deg is equivalent to "to right".
  iii) A value of 180deg is equivalent to "to bottom".

Syntax
background-image: linear-gradient(angle, color-stop1, color-stop2);
   
  ex : 
         background-image: linear-gradient(180deg, red, yellow);   //180deg -- to bottom

Using Multiple Color Stops
--------------------------------
ex :  background-image: linear-gradient(red, yellow, green);
       background-image: linear-gradient(to right, red,orange,yellow,green,blue,indigo,violet); //rainbow
  
Using Transparency
-----------------------
  ex :background-image: linear-gradient(to right, rgba(255,0,0,0), rgba(255,0,0,1));

Repeating a linear-gradient:
--------------------------------
ex :  background-image: repeating-linear-gradient(to right,red, yellow 10%, green 20%);
        background-image: repeating-linear-gradient(45deg,red,yellow 7%,green 10%);
        background-image: repeating-linear-gradient(90deg,red,yellow 7%,green 10%);
        background-image: repeating-linear-gradient(190deg,red,yellow 7%,green 10%);

b)Radial Gradients
.A radial gradient is defined by its center.
.To create a radial gradient you must also define at least two color stops.
.By default, shape is ellipse, size is farthest-corner, and position is center.


Syntax:
background-image: radial-gradient(shape size at position, start-color, ..., last-color);
.The shape parameter defines the shape. It can take the value circle or ellipse. 
 The default value is ellipse.

:shape size at position ---->ellipse|circle

  ex :
         background-image: radial-gradient(red, yellow, green);
         background-image: radial-gradient(red 5%, yellow 15%, green 60%);
         background-image: radial-gradient(circle, red, yellow, green);


Use of Different Size Keywords
------------------------------------
The size parameter defines the size of the gradient. It can take four values:

closest-side
farthest-side
closest-corner
farthest-corner

ex :
       background-image: radial-gradient(farthest-side at 60% 55%, red, yellow, black);
       background-image: radial-gradient(closest-corner at 60% 55%, red, yellow, black);
       background-image: radial-gradient(farthest-corner at 60% 55%, red, yellow, black);
       background-image: radial-gradient(farthest-corner at 60% 55%, red, yellow, black);


Using Repeating a radial-gradient :
----------------------------------------
ex :  
background-image: repeating-radial-gradient(red, yellow 10%, green 15%);



c)border-image
A shorthand property for setting all the border-image-* properties

 i)border-image :border-image-source border-image-slice border-image-width border-image-outset border-image-repeat;
.The border-image property allows you to specify an image to be used as the border around an element.

ex :  border-image : url(border.png) 30 round;
ex : border-image :none 100% 1 0 stretch;

a)border-image-source   :none|image|initial|inherit;    [def:none]
(Specifies the path to the image to be used as a border)
.The border-image-source property specifies the path to the image to be used as a border (instead of the normal border around an element).

Note :
If the value is "none", or if the image cannot be displayed, the border styles will be used.

b)border-image-slice  :number|%|fill|initial|inherit;    [def:100%]
 The border-image-slice property specifies how to slice the image specified by border-image-source. 
 The image is always sliced into   nine sections: four corners, four edges and the middle.
The "middle" part is treated as fully transparent, unless the fill keyword is set.


c)border-image-width        :number|%|auto|initial|inherit;  [def:1]
The border-image-width property can take from one to four values (top, right, bottom, and left sides)

d)border-image-outset    :length|number|initial|inherit;     [def:0]
.The border-image-outset property specifies the amount by which the border image area extends beyond the border box.
.The border-image-outset property can take from one to four values (top, right, bottom, and left sides). 


e)border-image-repeat   :stretch|repeat|round|initial|inherit;	 [def:stretch]
(Specifies whether the border image should be repeated, rounded or stretched)















