                             CSS

 1.CSS stands for Cascading Style Sheets
 2.CSS describes how HTML elements are to be displayed on screen   

   Syntax :
        Selector { Declaration};       //where Declaration --->(Property :value)

        Ex : h1{color:red};


  There are three methods of including CSS in an HTML document:

    Inline styles                — Using the style attribute in the HTML start tag.
    Embedded styles              — Using the <style> element in the head section of a document.
    External style sheets        — Using the <link> element, pointing to an external CSS file.     

  Ex :Inline styles 
    <h1 style="color: blueviolet;font-size: 28px;text-align: center;">
        INLINE Style :Using the style attribute in the HTML start tag.
    </h1>

 Ex :  Embedded styles 

 <!DOCTYPE html>
<html>
<head>
    <title>Embedded Style </title>
    <style>
      div{
          color: sienna;
          background-color:sandybrown;
          font-size: 48px;
          text-align: center;
      }
      pre{
        color: slateblue;
        font-size: 25px;
      }
    </style>
</head>
<body>
     <div>
        Embedded Style :
     </div>
     <pre>Using the style element in the head/body section of a document.</pre>
</body>
</html>  


  Ex:: External style sheets 

<!DOCTYPE html>
<html>
<head>
    <title>External Style sheet</title>
    <link rel='stylesheet' type='text/css' href='main.css'>
</head>
<body>
     <div>
        External Style :: Using the link element, pointing to an external CSS file.       
     </div>
    
</body>
</html>

main.css ::
----------
div{
    color:orange;
    font-size: 28px;
    text-align: center;
}