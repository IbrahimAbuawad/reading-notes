
## Name 5 Javascript UI Frameworks Other than React
* Sencha Ext JS
* Angular
* Vue
* Ember
* Svelte
* [Source SitePoint](https://www.sitepoint.com/javascript-ui-frameworks/)

## What's the difference between a framework and a library
* Libraries contain functions that can be called to perform a task
* Frameworks define how an application can be designed and the framework is what calls on the application code
* Libraries are still used, however, to be able to perform tasks
* [Source New relic Blog](https://blog.newrelic.com/engineering/best-javascript-libraries-frameworks/#:~:text=The%20key%20difference%20between%20JavaScript,than%20the%20other%20way%20around.)

## Define the Following Terms
* Rendering
  * Rendering is the "painting" of a web page onto the screen. Essentially rendering is the displaying of the code onto the webpage
* Templates
  * Templating refers to the "client side data binding method" used in Javascript. Templating often requires a template engine and this essentially outsources some of the work to the web browser.

## Preperation material
### The smallest React example looks like this:
```
ReactDOM.render(
  <h1>Hello, world!</h1>,
  document.getElementById('root')
);

```
### JSX
#### it is a syntax extension to JavaScript. We recommend using it with React to describe what the UI should look like.

#### React separates concerns with loosely coupled units called “components” that contain both.
#### React doesn’t require using JSX, but most people find it helpful as a visual aid when working with UI inside the JavaScript code. 
#### Example :
```
const name = 'Josh Perez';
const element = <h1>Hello, {name}</h1>;

ReactDOM.render(
  element,
  document.getElementById('root')
);

```

### rendeeing react
#### React elements are plain objects, and are cheap to create
#### Applications built with just React usually have a single root DOM node. 
#### React elements are immutable. Once you create an element, you can’t change its children or attributes

  * [Source Medium by Darlene Tate](https://medium.com/@BuildMySite1/javascript-templating-what-is-templating-7ff49d97db6b)
* State
  * State is the status of a program or an object and is used for coordinating code. For instance functions activating on state changes.
  * [Source Free Code Camp](https://www.freecodecamp.org/news/state-in-javascript-explained-by-cooking-a-simple-meal-2baf10a787ee/#:~:text=State%20describes%20the%20status%20of,instantly%20react%20to%20that%20change.)
