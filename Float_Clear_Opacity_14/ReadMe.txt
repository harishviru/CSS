i)Float   :left|right|none ;        [defVal:none]
.The CSS float property specifies how an element should float.
 The float property is used for positioning and formatting content 
 e.g. let an image float left to the text in a container     

 ii)Clear   :left|right|both|none;
.The clear property specifies what elements can float beside the cleared element and on which side.
.The most common way to use the clear property is after you have used a float property on an element.
.When clearing floats, you should match the clear to the float: 
  If an element is floated to the left, then you should clear to the left. 

  iii)Opacity
  .The opacity property specifies the opacity/transparency of an element.
  .The opacity property can take a value from 0.0 - 1.0. The lower value, the more transparent:
  .Default value is 1.0

ex :
  background: rgba(76, 175, 80, 0.3) /* Green background with 30% opacity */ 

iv)CSS Image Sprites

.An image sprite is a collection of images put into a single image.
.A web page with many images can take a long time to load and generates multiple server requests.
.Using image sprites will reduce the number of server requests and save bandwidth.

.By using background-position:width height;

ex:  background: url('img_navsprites.gif') 0 0;