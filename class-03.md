## HTML
### Lists
#### There are three types of HTML lists: 
##### 1. orderd 
##### 2. unorderd
##### 3. definition

#### Ordered lists use numbers
`<ol><li>list item</li></ol>`
#### Unordered lists use bullets
`<ul><li>list item</li></ul>`
#### Definition lists are used to define terminology
`<dl><dt>list item</dt></dl>`
*( dt ) contain the term being defined and ( dd ) is used to contain the definition.*
#### Lists can be nested inside one another.


### Boxex 
#### CSS treats each HTML element as if it has its own box.
#### You can use CSS to control the dimensions of a box.
#### You can also control the borders, margin and padding  for each box with CSS.
#### It is possible to hide elements using the display and  visibility properties.
####  Block-level boxes can be made into inline boxes, and  inline boxes made into block-level boxes.
#### Legibility can be improved by controlling the width of  boxes containing text and the leading .
#### CSS3 has introduced the ability to create image borders and rounded borders.

#### we can use box-shadow and it has 4 properties :
##### 1. Horizontal offset
##### 2. Vertical offset
##### 3. Blur distance
##### 4. Spread of shadow

#### The property requires three pieces of information about **Border-image**:
##### 1. The URL of the image 
##### 2. Where to slice the image
##### 3. What to do with the straight


## JavaScript
### Basic JavaScript Instructions
#### Arrays are special types of variables that store more  than one piece of related information. 
##### Example : 
###### let ArrayName = [ "Ahmad" , "Ibrahim", 30 , 23 ];

#### ach item in an array is automatically given a number  called an index. This can be used to access specific items in the array.
*Ahmad > 1 , Ibrahim > 2 , 30 > 3 , 23 > 4*

#### we can ACCESSING ITEMS IN AN ARRAY :
*ArrayName[2] >> 2 is the index of array*


### Decisions and Loops(switch)
#### switch statements allow you to compare a value against possible outcomes (and also provides a default option if none match). 
#### Data types can be coerced from one type to another. 
#### All values evaluate to either truthy or falsy. 
#### types of loops :
##### 1. For 
##### 2. while 
##### 3. Do while 

##### Example of for Loop : 
`for(var i = 0 ; i < 10 ; i++){document.write(i);}`.
##### *var i=0 initialization , i<10 condition , i++ update*

##### Example of while loop :
` while (i < 10) { msg += i + ' x 5 = ' + (i * 5) + '<br I>'; i++; }`
 
##### Example of switch loop :
` switch (level){ case 'one' : title = 'level 1';break;}`
*and continue the above example with another case & title .. and so on *

#### The key difference between  a **while** loop and a **do while** loop is that the statements in  the code block come before the condition. This means that those  statements are run once whether or not the condition is met. 


