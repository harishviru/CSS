                                 Animations
                                 ==========
 .An animation lets an element gradually change from one style to another.
 .You can change as many CSS properties you want, as many times you want.
 .To use CSS animation, you must first specify some keyframes for the animation.
 .Keyframes hold what styles the element will have at certain times.

 @keyframes:
.When you specify CSS styles inside the @keyframes rule, 
the animation will gradually change from the current style to the new  style at certain times.
.To get an animation to work, you must bind the animation to an element.
.If the animation-duration property is not specified, no animation will occur, because the default value is 0s (0 seconds). 

In the example above we have specified when the style will change by using the keywords "from" and "to" (which represents 0% (start) and 100% (complete)).
@keyframes example {
  from {background-color: red;}
  to {background-color: yellow;}
}

i)animation-name 	    :keyframename|none;                          [defVal:none]
Specifies the name of the @keyframes animation
ex :  animation-name: example;

ii)animation-duration 	 :time|initial|inherit;                           [defVal:0]
Specifies how long time an animation should take to complete one cycle
 ex :  animation-duration: 3s;

iii)animation-timing-function 	                                         [defVal:ease]
:linear|ease|ease-in|ease-out|ease-in-out|step-start|step-end|steps(int,start|end)|cubic-bezier(n,n,n,n);
Specifies the speed curve of the animation
 ex :animation-timing-function :linear

iv)animation-delay 	  : time|initial|inherit;                [defVal :0]                   
Specifies a delay for the start of an animation
ex :  animation-delay: 2s;

v)animation-iteration-count  :number|infinite|initial|inherit;       [defVal:1]
The animation-iteration-count property specifies the number of times an animation should be played.
ex :animation-iteration-count :3;

vi)animation-direction     :normal|reverse|alternate|alternate-reverse|initial|inherit;    [defVal:normal]
The animation-direction property defines whether an animation should be played forwards, backwards or in alternate cycles.
ex :animation-direction ;reverse;

vii)animation-fill-mode  :none|forwards|backwards|both|initial|inherit;    [defVal:none]
.The animation-fill-mode property specifies a style for the element when the animation is not playing 
  (before it starts, after it ends, or both).
.CSS animations do not affect the element before the first keyframe is played or after the last keyframe is played. 
The animation-fill-mode property can override this behavior. 
 ex:  animation-fill-mode: forwards;

viii)animation-play-state    :paused|running|initial|inherit;           [defVal:running]
The animation-play-state property specifies whether the animation is running or paused.
ex :animation-play-state :paused;

Animation short Hand property :
 animation: name duration timing-function delay iteration-count direction fill-mode play-state;
 ex :animation: example 2s ease 3s 2 reverse forwards running;














