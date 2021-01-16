i)text-overflow    :clip|ellipsis|string
The text-overflow property specifies how overflowed content that is not displayed should be signaled to the user. It can be clipped, display an ellipsis (...), or display a custom string.
Both of the following properties are required for text-overflow:

    white-space: nowrap;
    overflow: hidden;
    
ii)overflow     :visible |hidden |scroll|auto  [DefVal :visible]
.The overflow property specifies whether to clip the content or to add scrollbars 
when the content of an element is too big to fit in the specified area.

Note: The overflow property only works for BLOCK elements with a specified height.

i)overflow-x	
(Specifies what to do with the left/right edges of the content if it overflows the element's content area)

ii)overflow-y	
(Specifies what to do with the top/bottom edges of the content if it overflows the element's content area)
