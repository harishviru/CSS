                   Multiple Columns
                   ===============
.The CSS multi-column layout allows easy definition of multiple columns of text - just like in newspapers.

i)column-count    :number|auto|initial|inherit;         [DefVal:auto]	
Specifies the number of columns an element should be divided into
ex :column-count :3;

ii)column-width    :auto|length|initial|inherit           [defVal:auto]
The column-width property specifies the column width.
.The number of columns will be the minimum number of columns needed to show all the content across the element.
 ex :column-width:200px;

iii)columns              :auto|column-width column-count|initial|inherit;    [defVal:auto auto]    (Short Hand property )
The columns property is a shorthand property for column-width column-count

syntax :
       columns :column-width column-count;
ex : columns:200px 3;

iv)column-span           : none|all|initial|inherit;     [Defval:none]
The column-span property specifies how many columns an element should span across.
ex :column-span :all;

v)column-fill          :balance|auto|initial|inherit;       [defVal:balance]
The column-fill property specifies how to fill columns, balanced or not.
ex :column-fill :auto;

vi) column-gap         : length|normal|initial|inherit;   [DefVal:normal]
The column-gap property specifies the gap between the columns.
ex ;column-gap :40px;



vii)column-rule-width 	 :medium|thin|thick|length|initial|inherit;      [defVal:medium]
Specifies the width of the rule between columns
ex :column-rule-width:medium;

viii)column-rule-style   : none|hidden|dotted|dashed|solid|double|groove|ridge|inset|outset|initial|inherit;  [defVal:none]
The column-rule-style property specifies the style of the rule between columns.
ex :column-rule-style :dotted;

ix)column-rule-color   :color|initial|inherit;
The column-rule-color property specifies the color of the rule between columns.
 ex :column-rule-color:blue;

x)column-rule   (Short Hand property )
The column-rule property sets the width, style, and color of the rule between columns.

syntax :
      column-rule :column-width column-style column-color










