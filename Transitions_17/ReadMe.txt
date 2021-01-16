
                           CSS Transitions

.CSS transitions allows you to change property values smoothly, over a given duration.
. If the duration part is not specified, the transition will have no effect, because the default value is 0

CSS transitions properties :
i)transition-property
ii)transition-duration
iii)transition-timing-function
iv)transition-delay
v)transition

i)transition-property 	 :none|all|property|initial|inherit;  [defVal:all]
Specifies the name of the CSS property the transition effect is for
ex :  transition-property: width;

ii)transition-duration 	  : time|initial|inherit;   [defVal:0s]
Specifies how many seconds or milliseconds a transition effect takes to complete
ex :   transition-duration: 5s;

iii)transition-timing-function  
           : linear|ease|ease-in|ease-out|ease-in-out|step-start|step-end|steps(int,start|end)|cubic-bezier(n,n,n,n);	
Specifies the speed curve of the transition effect
ex :transition-timing-function: linear;                 [defVal:ease]

iv)transition-delay 	 :time|initial|inherit;   [defVal:0s]
Specifies a delay (in seconds) for the transition effect
ex :  transition-delay: 2s;

v)transition
.Short hand property :
           transition: property duration timing-function delay; //defVal :all 0s ease 0s
    ex : transition: width 2s ease 2s;

