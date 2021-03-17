## JavaScript
### Functions, Methods, and Objects
#### Functions let you group a series of statements together to perform a  specific task. If different parts of a script repeat the same task, you can  reuse the function (rather than repeating the same set of statements). 
##### Example : 
##### *function updateMessage() {var el = document.getElementByld('message'}; el .textContent = msg;*

![Function component](https://res.cloudinary.com/practicaldev/image/fetch/s--OKK_5-yp--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://raddevon.com/wp-content/uploads/2019/07/function-declaration-diagram-1024x282.png)

##### xample of calling a function :
`sayHello();`
##### if it has an information :
`sayHello('Width','height');`

#### Functions allow you to group a set of related statements together that represent a single task. 
#### Functions can take parameters (informatiorJ required to do their job) and may return a value.
###### function('String',Number){any thing you want}

#### An object is a series of variables and functions that represent something from the world around you.
##### Example of object:
`let variables = {'first':10 , 'second':20} ` 
#### In an object, variables are known as properties of the object; functions are known as methods of the object. 
#### Web browsers implement objects that represent both the browser window and the document loaded into the browser window. 

#### JavaScript also has several built-in objects such as :
##### 1. 
##### 2.  
##### 3. 
##### 4. 

#### Arrays and objects can be used to create complex data sets .
###### {accom: 460, food: 20, phone: 20} 


### DOM
#### The browser represents the page using a DOM tree. 
#### DOM trees have four types of nodes:
##### + document nodes.
##### + element nodes.
##### + attribute nodes. 
##### + and text nodes.

#### You can select element nodes by their id or cl ass attributes, **by tag name**, or **using CSS selector syntax**. 
#### Whenever a DOM query can return more than one node, it will always return a Nadel i st. 
#### From an element node, you can access and update its content using properties such as textContent and i nnerHTML or using DOM manipulation techniques. 
##### Example:
*let el = document .querySel ector('li .hot ' };*

#### An element node can contain multiple text nodes and 
#### child elements that are siblings of each other.

 ![DOM](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/08/Js-Dom-Tree.png)
 
#### In older browsers, implementation of the DOM is inconsistent (and is a popular reason for using jQuery). 
#### Browsers offer tools for viewing the DOM tree . 