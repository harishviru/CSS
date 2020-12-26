                    CSS Selectors

 CSS selectors are used to "find" (or select) the HTML elements you want to style.

 We can divide CSS selectors into five categories:

 
    1. Simple selectors           (select elements based on name, id, class)
    2. Combinator selectors       (select elements based on a specific relationship between them)
    3. Attribute selectors        (select elements based on an attribute or attribute value)
    4. Pseudo-elements selectors  (select and style a part of an element)
    5. Pseudo-class selectors     (select elements based on a certain state)
==============================================================================================

#1.Simple selector  : (select elements based on name, id, class)
     i)Universal Selector   (*)
     ii)Element Type Selectors (p,div,h1,h2....etc; all HTML elements)
     iii)Id Selectors  (#)
     iv)Class Selectors  (.)

  i)Universal Selector   (*)  [if you want to select all Html elements,then we can use * symbol]
  * {
    margin: 0;
    padding: 0;
  } 

 ii)Element Type Selectors (p,div,h1,h2....etc; all HTML elements)
   div {
      color: green;
   }

 iii)Id Selectors  (#) [The id(#) selector is used to define style rules for a single or unique element.]
    
 #success {
      color: green;
   }

iv)Class Selectors  (.)
   The class selectors can be used to select any HTML element that has a class(.) attribute.
   .success {
      color: green;
   }
   div.success {
     color: green;
   }

---------------------------------*--------------------------------*--------------------------
2. Combinator selectors ::      (select elements based on a specific relationship between them)

#A combinator is something that explains the relationship between the selectors.
There are four different combinators in CSS:

    i)descendant selector                      (space)
    ii)child selector                           (>)
    iii)adjacent sibling selector               (+)
    iv)general sibling selector                 (~)


i)descendant selector  (space)

#The descendant selector matches all elements that are descendants of a specified element.
div p {
  background-color: yellow;
}

 ii)child selector     (>)

 #The child selector selects all elements that are the children of a specified element.
 div > p {
  background-color: yellow;
}

 iii)adjacent sibling selector   (+) [select one adjacent element ]

 #The adjacent sibling selector is used to select an element that is directly after another specific element.
 #Sibling elements must have the same parent element, and "adjacent" means "immediately following".
div + p {
  background-color: yellow;
}

iv)general sibling selector   (~)  [select all adjacent element ]

#The general sibling selector selects all elements that are siblings of a specified element.
div ~ p {
  background-color: yellow;
}


---------------------------------------------------------------------------------------------
 3. Attribute selectors  (select elements based on an attribute or attribute value)
Selector 	             Example 	            Example description
[attribute] 	      [target] 	              Selects all elements with a target attribute
[attribute=value] 	[target=_blank] 	      Selects all elements with target="_blank"
[attribute~=value] 	[title~=flower] 	      Selects all elements with a title attribute containing the word "flower"
[attribute|=value] 	[lang|=en] 	            Selects all elements with a lang attribute value starting with "en"
[attribute^=value] 	a[href^="https"] 	      Selects every <a> element whose href attribute value begins with "https"
[attribute$=value] 	a[href$=".pdf"] 	      Selects every <a> element whose href attribute value ends with ".pdf"
[attribute*=value] 	a[href*="google"] 	    Selects every <a> element whose href attribute value contains the substring "google"

It is possible to style HTML elements that have specific attributes or attribute values.

i)[attribute] 
The [attribute] selector is used to select  all elements if it is having attribute.
 [target] {                            
  background-color: green;
 }

ii)[attribute=value] 
The [attribute="value"] selector is used to select elements with a specified attribute and value.
a[target="_blank"] {
  background-color: brown;
}

iii)[attribute~=value] // symbol(~)=tilde  
The [attribute~="value"] selector is used to select elements with an attribute value 
containing a specified word.

[title~="flower"] {
  background-color: brown;
}
The example above will match elements with 
title="flower", title="summer flower", and title="flower new",
but not title="my-flower" or title="flowers".

iv)[attribute|=value]    // symbol (|)=vertical bar
The [attribute|="value"] selector is used to select elements with the specified attribute starting with the specified value.
[class|="top"] {
  background: yellow;
}
Note: The value has to be a whole word, either alone, like class="top", or followed by a hyphen( - ), like class="top-text"! 
       but not class="top header" or class="topheader"  or class="top_header"
 
v)[attribute^=value]   //symbol(^)=caret 
The [attribute^="value"] selector is used to select elements whose attribute value begins with a specified value.

[class^="top"] {
  background: brown;
}

vi)[attribute$=value]   //symbol($)=dolar 
The [attribute$="value"] selector is used to select elements whose attribute value ends with a specified value.

[class$="top"] {
  background: brown;
}

vii)[attribute*=value]  //symbol(*)=start
The [attribute*="value"] selector is used to select elements whose attribute value contains a specified value.

[class*="top"] {
  background: brown;
}
-----------------------------------------------------------------------------------------------
4. Pseudo-elements selectors  (select and style a part of an element)

For example, it can be used to:

    Style the first letter, or line, of an element
    Insert content before, or after, the content of an element

Syntax

The syntax of pseudo-elements:

selector::pseudo-element {
  property: value;
}

All CSS Pseudo Elements


Selector            	Example 	           Example description
::after              	p::after 	        Insert something after the content of each <p> element
::before 	            p::before 	      Insert something before the content of each <p> element
::first-letter 	      p::first-letter 	Selects the first letter of each <p> element
::first-line        	p::first-line 	  Selects the first line of each <p> element
::selection 	        p::selection 	    Selects the portion of an element that is selected by a user


i)::first-letter 
The ::first-letter pseudo-element is used to add a special style to the first letter of a text.

p::first-letter {
  color: #ff0000;
}

ii)::first-line 
The ::first-line pseudo-element is used to add a special style to the first line of a text.

p::first-line {
  color: #ff0000;
}

iii)::after 
The ::after pseudo-element can be used to insert some content after the content of an element.
h1::after {
  content: "****";
}

iv)::before 
The ::before pseudo-element can be used to insert some content before the content of an element.
h1::before {
  content: "****";
}

v)::selection 
The ::selection pseudo-element matches the portion of an element that is selected by a user.

p::selection {
  color: red;
}

-----------------------------------------------------------------------------------------------
5. Pseudo-class selectors     (select elements based on a certain state)

Syntax

The syntax of pseudo-classes:
selector:pseudo-class {
  property: value;
}

All CSS Pseudo Classes

i)    :root

ii)   :hover
iii)  :focus

iv)   :disabled
v)    :enabled

vi)   :optional
vii)  :required

viii) :out-of-range
ix)   :in-range

x)    :valid
xi)   :invalid

xii)   :read-only
xiii)  :read-write
xiv)   :checked

xv)    :link
xvi)   :active
xvii)  :visted

xviii):empty
xix)  :lang(language)
xx)   :not(selector)
xxi)  :target


xxii)     :first-child
xxiii)    :first-of-type

xxiv)     :last-child
xxv)      :last-of-type

xxvi)     :nth-child(n)
xxvii)    :nth-of-type(n)

xxviii)   :nth-last-child(n)
xxix)     :nth-last-of-type(n)

xxx)      :only-of-type
xxxi)     :only-child
