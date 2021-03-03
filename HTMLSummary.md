## PROCESS & Design
#### Site maps allow you to plan the structure of a site.
#### You can differentiate between pieces of information using size, color, and style.
#### Wireframes : allow you to organize the information that will need to go on each page.
#### Every website should be designed for the target audience—not just for yourself or the site owner. It is therefore very important to understand who your target audience is.
![wireFrame](https://th.bing.com/th/id/R9fc099ab5a8993f144ba3e405d92d0db?rik=GQteKF%2fBoRnSLQ&riu=http%3a%2f%2flivianieves.com%2f221%2fclasses%2fclass3%2fwireframe4final-template.jpg&ehk=XCgNAhbDOrLPcxgVfFoX6K7%2fT7xmaDNQrMlgixkVELI%3d&risl=&pid=ImgRaw)


## Structure of HTML
#### HTML uses tags (characters that sit inside angled brackets) to give the information they surround special meaning.
##### Example :
##### <>content</>

#### Tags usually come in pairs. The opening tag denotes the start of a piece of content; the closing tag denotes the end.
##### Example :
`<h1></h1>`
#### Opening tags can carry attributes, which tell us more about the content of that element.
##### Example : href 
`<a href=""></a>` 
#### Attributes require a name and a value
##### Example : 
`<a href="Link"></a>` 


## HTML5 layout
#### The new HTML5 elements indicate the purpose of different parts of a web page and help to describe its structure.
#### the HTML5 support using 
##### Examples of usage include:
1. Images
2. Videos
3. Graphs
4. Diagrams
5. Code samples
6. Text that supports the main

#### Older browsers that do not understand HTML5 elements need to be told which elements are block-level elements.
#### To make HTML5 elements work in Internet Explorer 8 (and older versions of IE), extra JavaScript is needed, 
##### Example of HTML5 :
`<body> 
<div class="wrapper">
 <header> 
 <h1>Yoko's Kitchen</h1> 
 <nav> 
  <ul> 
    <li><a href="" class="current">home</a></li> 
    <li><a href="">classes</a></li> 
    <li><a href="">catering</a></li> 
    <li><a href="">about</a></li> 
    <li><a href="">contact</a></li> 
  </ul> 
 </nav> 
</header> 
</body>`

## Extra Markup
#### DOCTYPES tell browsers which version of HTML you are using.
#### You can add comments to your code between the markers.
##### Example :
`<!--add your comment here-->`
#### The id and class attributes allow you to identify particular elements.
##### Example :
`<h1 class="className" id="idName"></h1>`
#### Escape characters are used to include special characters in your pages such as <, >, and ©.
#### The <div> and <span> elements allow you to group block-level and inline elements together.