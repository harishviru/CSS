CSS Outline Properties

An outline is a line that is drawn around elements, OUTSIDE the borders, to make the element "stand out". 

CSS has the following outline properties:
    outline-style
    outline-color
    outline-width
    outline-offset
    outline


i)outline-style                                 :dotted,dashed,solid,double,groove,ridge,inset ,outset ,none,hidden.

ii)outline-width                                : thin, medium, or thick,length

The outline-width property specifies the width of the outline, and can have one of the following values:

     thin, medium, or thick

The width can be set as a specific size (in px, pt, cm, em, etc) or by using one of the three pre-defined values: :

  outline-width  : 25px 10px 4px 35px; /* 25px top, 10px right, 4px bottom and 35px left */


iii)outline-color                             :red,blue....etc 

The outline property is a shorthand property for the following individual outline properties:

    outline-width
    outline-style (required)
    outline-color

 p {
  outline:5px solid red;
}

iv)outline-offset                                  :length (ex :15px)
Specifies the space between an outline and the edge or border of an element
