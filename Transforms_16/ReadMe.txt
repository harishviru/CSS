                   Transforms
                   ----------
 2D  & 3D Transforms:
 ====================
 .CSS transformations allow you to translate,rotate,scale,and skew elements.
 .A transformation is an effect that lets an element change shape,size and position

CSS 2D Transforms Methods :
    i)   translate(),translateX(),translateY()
    ii)  rotate()

    iii) scale(), scaleX(),scaleY()
 
    iv) skew(), skewX(),skewY()

    v)  matrix()

i)translate        :translate(x,y) 
The translate() method moves an element from its current position (according to the parameters given for the X-axis and the Y-axis).
ex :   transform: translate(50px, 100px);

ii)rotate        :rotate(deg)
The rotate() method rotates an element clockwise or counter-clockwise according to a given degree.
ex :   transform: rotate(20deg);           [negative val :anti or counter-clockwise]

iii) scale() ,scaleX(),scaleY()
The scale() method increases or decreases the size of an element (according to the parameters given for the width and height).
The scaleX() method increases or decreases the width of an element.
The scaleY() method increases or decreases the height of an element.
ex :    transform: scale(2, 3);
        transform: scaleX(2);
        transform: scaleY(2);

iv) skew(), skewX(),skewY()
The skew() method skews an element along the X and Y-axis by the given angles.
The skewX() method skews an element along the X-axis by the given angle.
The skewY() method skews an element along the Y-axis by the given angle.
ex :     transform: skew(20deg, 10deg);
         transform: skewX(20deg);
         transform: skewY(20deg);

v) matrix()
The matrix() method combines all the 2D transform methods into one.
syntax :
   matrix(scaleX(),skewY(),skewX(),scaleY(),translateX(),translateY())

  ex: transform: matrix(1, -0.3, 0, 1, 0, 0);


 CSS transform property supports 3D transformation methods:
i)translate3d(x,y,z) ,translateX(x),translateY(y),translateZ(z)
The translate() method moves an element from its current position (according to the parameters given for the X-axis and the Y-axis,Z-axis)
ex :   transform: translate(50px, 100px,40px);

ii)rotate3d(x,y,z,angle) ,rotateX(), rotateY(), rotateZ()
Defines a 3D rotation
ex :rotate3d(1,3,5,45deg)

iii)scale3d(x,y,z), scaleX(),scaleY(),scaleZ();
Defines a 3D scale transformation
ex :scale3d(2,3,4)

iv)perspective(n)  :perspective: length|none;
Defines a perspective view for a 3D transformed element.
The perspective property is used to give a 3D-positioned element some perspective.
The perspective property defines how far the object is away from the user. 
So, a lower value will result in a more intensive 3D effect than a higher value.
ex :     perspective: 150px;

v)matrix3d
Defines a 3D transformation, using a 4x4 matrix of 16 values
matrix3d(a1, b1, c1, d1, a2, b2, c2, d2, a3, b3, c3, d3, a4, b4, c4, d4)
a1 b1 c1 d1 a2 b2 c2 d2 a3 b3 c3 d3
    Are <number>s describing the linear transformation.
a4 b4 c4 d4
    Are <number>s describing the translation to apply. 

=====0====
transform-style :flat|preserve-3d  [def:flat]
The transform-style property specifies how nested elements are rendered in 3D space.

Note: This property must be used together with the transform property.




