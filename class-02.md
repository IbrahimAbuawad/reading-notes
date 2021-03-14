## HTML
### Text
#### HTML elements are used to describe the structure of  the page (e.g. headings, subheadings, paragraphs).
##### Example of Heading :
*h1 , h2 , h3 , h4 , h5 , h6*
##### Example of paragraph :
`<p>Content</p>`

#### the **<del>** element can show text that has been deleted from it.
##### Example of del tag :
`<del>content</del> `
###### it will be ~content~ 

#### **<br>** the browser will automatically show each new paragraph or heading  on a new line. 
#### The **<sup>** element is used  to contain characters that  should be superscript
#### They also provide semantic information (e.g. where  emphasis should be placed, the definition of any acronyms used, when given text is a quotation).

### Introducing CSS
#### CSS treats each HTML element as if it appears inside  its own box and uses rules to indicate how that  element should look.
#### Rules are made up of selectors (that specify the  elements the rule applies to) and declarations (that  indicate what these elements should look like).
#### Different types of selectors allow you to target your  rules at different elements.
#### Declarations are made up of two parts :
##### 1. the properties of the element that you want to change.
##### 2. the values of those properties .

#### many selector in css :
##### 1. Universal Selector : ***{}**
##### 2. Type Selector : **h1 , h2 , h3 {}**
##### 3. class selector **.cont{}**
##### 4. id selector : **#paragraph{}**


## JavaScript 
### basic JS instruction 
#### A script is made up of a series of statements. Each  statement is like a step in a recipe. 
#### Scripts contain very precise instructions. For example,  you might specify that a value must be remembered before creating a calculation using that value. 
#### Variables are used to temporarily store pieces of  information used in the script. 
##### Example :
###### let variableName = "String"; 

#### Arrays are special types of variables that store more  than one piece of related information. 
##### Example : 
###### let ArrayName = [ "Ahmad" , "Ibrahim", 30 , 23 ];

#### JavaScript distinguishes between numbers **(0-9)**, strings **(text)**, and Boolean values **(true or false)**.

#### Expressions evaluate into a single value.

### Decisions and Loops
#### you can evaluate a situation by comparing one value in the script to what you wxpect it might be
#### the operators is :
##### 1. == equal to.
##### 2. != Not equal to.
##### 3. !== strict equal to .
##### 4. === Strict not equal to .
##### 5. > Greater Than .
##### 6. < Less than .
##### 7. >= greater than or equal to .
##### 8. <= Less Than or equal to .

#### Comparision operators usally return single values of **True** or **False**.

##### Example :
`( ( 5 < 2 ) && ( 2 >= 3 ) )`.

#### the coparision operators is :
##### 1. && logical And .
##### 2. || Logical Or .
##### 3. Logical Not .


#### Loops check a condition . if it returns true , a code block will run , then the condition will be checked again and if it still returns true the code block will run again until it return false.

#### types of loops :
##### 1. For 
##### 2. while 
##### 3. Do while 

##### Example of for Loop : 
`for(var i = 0 ; i < 10 ; i++){document.write(i);}`.
##### *var i=0 initialization , i<10 condition , i++ update*

##### Example of while loop :
` while (i < 10) { msg += i + ' x 5 = ' + (i * 5) + '<br I>'; i++; }`