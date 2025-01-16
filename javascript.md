Javascript Notes

:modules: - an external file that contains reusable code that can be imported into other
javascript files. Write reusable code for man different apps. Can contain
variables, classes, functions ... and more. Introduced as part of 
ECMASCRIPT 2015 Update.
- before importing the external file into another javascript file, make sure
to add the keyword "export" to any variables, classes and functions you wish
to use.
- to import the external file make sure you add the module type when adding
the source in the hml file.
```
<script type="module" src="/src/main.js"></script>
```
- then import the external file into another javascript file. You can now use
- the exported variables, classes and functions from the external file.
```
import {} from './external.js';
```

:synchronous: - executes line by line consequetively in a sequencial manner. Code
that waits for an operation to complete.

:asynchronous: - Allows multiple operation to be performed concurrently without
waiting. Doesn't block the execuation flow and allows the program to continue.
(I/O operations, network requests, fetching data)
Handled with: Callbacks, Promises, Async/Await
```
function func1(callback) {
  setTimeout(() => {
      console.log("task 1");
      callback();
  }, 3000)
}

function func2() {
  console.log("task 2");
  console.log("task 3");
  console.log("task 4");
}

func1(func2);
```

:error: - an object that is created to represent problem thats occurs. Occur 
often with user input or establishing connection.

:try: - encloses code that might potentially cause an error.
:catch: - catch and handle any thrown errors from try {}
:finally: - (optional) Always executes. Used mostly for clean up.
ie. close files, close connections, release resource
```
try {
  console.log(x);
  // network errors
  // promise rejection
  // security errors
}
catch(error) {
  // console.log(error);
  console.error(error); // recommended to use console.error
}
```

:DOM: - document object model
object{} that represents the page you see in the web browser and provides you
with an API to interact with it. Web browser constructs the DOM when it loads
an HTML document, and structures all the elements in a tree-like representation.
Javascript can access the DOM to dynamically change the content, structure,
and style of the web page.

:element_selector: - methods used to target and manipulate HTML elements.
They allow you to select one or multiple HTML elements from the DOM
1. document.getElementById() // element or null
2. document.getElementsByClassName() // html collection
3. document.getElementsByTagName() // html collection
4. document.querySelector() // element or null
5. document.querySelectorAll() // nodelist

- html collection don't have forEach() function but you can typecast it into
an array.(ie. Array.from(htmlCollection).forEach(html => {do something}))
- nodelist are static. html collection are live.
- you can use forEach() on nodelist.

:css_property:
- accessing css properties through the DOM has a camelCase naming conventing.
- in css file, the properties have a hypenated naming convention(ie. font-size).

:dom_navigation: - the process of navigating through the structure of an HTML
document using javascript.
- .firstElementChild
- .lastElementChild
- .nextElementSibling
- .previousElementSibling
- .parentElement
- .children

