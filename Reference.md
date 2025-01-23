#Bryan Lorenzo's Reference Notes

##Card Format
id:
source:
tag:


id: 2025-01-23c
source:
tag: #vocabulary
>ambivalence - n. the state of having mixed feelings or contraditory ideas 
>about something or someone.
>
>codger - an elderly man, especially one who is old-fashion or eccentric.
>
>palindrome - a word, phrase or sequence that reads the same backward as forward.
>
>cot - n. a camp bed, particularly a portable, collapsible one.
>
>schoolmarm- n. a schoolmistress(typically used with a reference to a woman
>regarded as prim, strict, and brisk in manner).

id: 2025-01-23b
source: https://www.cyberciti.biz/faq/debian-ubuntu-linux-delete-old-kernel-images-command/
tag: #linux, #apt, #autoremove
>On newer system all obsolete kernels and headers should automatically be 
>flagged as no more needed, and thus can be purged with the following single 
>command: sudo apt --purge autoremove

id: 2025-01-23a
source: https://unix.stackexchange.com/questions/20460/how-do-i-do-a-ls-and-then-sort-the-results-by-date-created
tag: #linux, #ls
>to list files by creation/birth date/time, you can use:
>ls -t --time=birth
>add -r to reverse the order

id: 2025-01-22g
source: https://youtu.be/dUPBeEWH418?si=qMzJf4ZJAEPPjcT0
tag: #3d_printing, #tree_generator

id: 2025-01-22f
source: https://youtu.be/0XYwtub9bJE?si=ROQMVEv-00rl1Bez
tag: #3d_printing, #sun_tracking

id: 2025-01-22e
source: https://youtu.be/uJiauHFUbn8?si=R9rN16IcL5x-qchZ
tag: #3d_printing, #string_pulley

id: 2025-01-22d
source: https://youtu.be/TQiLLcumqDw?si=ffpC3ruYUtu5NxJl
source: https://youtu.be/jM5Sy5Eu9pA?si=Qi9iv9lKVh7KjVds
tag: #3d_printing, #rolling_contact_bearing
>- an alternative to ball bearing for robotic movement and other application.
>- works similar to bones and tendons in a bionic level.

id: 2025-01-22c
source:
tag: #c_programming
>- middle level language
>
>1. C is not an object oriented language. (procedural)
>2. C++ is an object oriented extension of C.
>3. C is a difficult language for beginners.
>
>
>:c_variables:
>```
>int x = 10; // declaration + initialization
>float pi = 3.14; // floating point number
>char grade = 'B'; // single character
>char name[] = "Bryan" // array of characters;
>
>printf("Number %d\n", x);
>printf("Pi is %f\n", pi);
>printf("Your grade is %c\n", grade);
>printf("Hello %s\n", name);
>```

id: 2025-01-22b
source:
tag: #coding_game
>:coding_game:
>- robocode https://robocode.sourceforge.io/
>- codeingame https://www.codingame.com/start/
>- codemonkey https://www.codemonkey.com/
>- codecombat https://codecombat.com/
>- screeps https://screeps.com/
>- tis-100
>- human resource machine
>- duskers
>- flexbox defense
>- elevator saga

id: 2025-01-22a
source:
tag: #dyneema
>- a strong fiber used for fishing line. does not stretch.

id: 2025-01-20b
source:
tag: #idiom
>"a day late and a dollar short" - someone is too late and doesn't have the
>resource to take advantage of an opportunity.

id: 2025-01-20a
source:
tag: #javascript
>:modules: - an external file that contains reusable code that can be imported into other
>javascript files. Write reusable code for man different apps. Can contain
>variables, classes, functions ... and more. Introduced as part of 
>ECMASCRIPT 2015 Update.
>- before importing the external file into another javascript file, make sure
>to add the keyword "export" to any variables, classes and functions you wish
>to use.
>- to import the external file make sure you add the module type when adding
>the source in the hml file.
>```
><script type="module" src="/src/main.js"></script>
>```
>- then import the external file into another javascript file. You can now use
>- the exported variables, classes and functions from the external file.
>```
>import {} from './external.js';
>```
>
>:synchronous: - executes line by line consequetively in a sequencial manner. Code
>that waits for an operation to complete.
>
>:asynchronous: - Allows multiple operation to be performed concurrently without
>waiting. Doesn't block the execuation flow and allows the program to continue.
>(I/O operations, network requests, fetching data)
>Handled with: Callbacks, Promises, Async/Await
>```
>function func1(callback) {
>  setTimeout(() => {
>      console.log("task 1");
>      callback();
>  }, 3000)
>}
>
>function func2() {
>  console.log("task 2");
>  console.log("task 3");
>  console.log("task 4");
>}
>
>func1(func2);
>```
>
>:error: - an object that is created to represent problem thats occurs. Occur 
>often with user input or establishing connection.
>
>:try: - encloses code that might potentially cause an error.
>:catch: - catch and handle any thrown errors from try {}
>:finally: - (optional) Always executes. Used mostly for clean up.
>ie. close files, close connections, release resource
>```
>try {
>  console.log(x);
>  // network errors
>  // promise rejection
>  // security errors
>}
>catch(error) {
>  // console.log(error);
>  console.error(error); // recommended to use console.error
>}
>```
>
>:DOM: - document object model
>object{} that represents the page you see in the web browser and provides you
>with an API to interact with it. Web browser constructs the DOM when it loads
>an HTML document, and structures all the elements in a tree-like representation.
>Javascript can access the DOM to dynamically change the content, structure,
>and style of the web page.
>
>:element_selector: - methods used to target and manipulate HTML elements.
>They allow you to select one or multiple HTML elements from the DOM
>1. document.getElementById() // element or null
>2. document.getElementsByClassName() // html collection
>3. document.getElementsByTagName() // html collection
>4. document.querySelector() // element or null
>5. document.querySelectorAll() // nodelist
>
>- html collection don't have forEach() function but you can typecast it into
>an array.(ie. Array.from(htmlCollection).forEach(html => {do something}))
>- nodelist are static. html collection are live.
>- you can use forEach() on nodelist.
>
>:css_property:
>- accessing css properties through the DOM has a camelCase naming conventing.
>- in css file, the properties have a hypenated naming convention(ie. font-size).
>
>:dom_navigation: - the process of navigating through the structure of an HTML
>document using javascript.
>- .firstElementChild
>- .lastElementChild
>- .nextElementSibling
>- .previousElementSibling
>- .parentElement
>- .children

id: 2025-01-19a
source:
tag: #data_structure_and_algorithm
>:big_O_notation: "How code slows as data grows." 
>1. Describes the performance of an algorithm as the amount of data increases.
>2. Machine independent (# of steps to completion)
>3. Ignore smaller operations O(n + 1) -> 0(n)
>
>example:  O(1) - constant time
>          O(n) - linear time
>          O(log n)
>          O(n^2)
>
>n = amount of data (it's a variable like x)
>
>O(1) - constant time
>* random access of an element in an array
>* inserting at the beginning of linkedlist
>
>O(log n) - logarithmic time
>* binary search
>
>O(n) - linear time
>* looping through elements in an array
>* searching through a linkedlist
>
>O(n log n) - quasilinear time
>* quicksort
>* mergesort
>* heapsort
>
>O(n^2) - quadratic time
>* insertion sort
>* selection sort
>* bubblesort
>
>O(n!) - factorial time
>* traveling salesman problem
>
>:stacks:
>- last in first out(LIFO).
>- push() to put or add a value at the end of the stack
>- pop() to remove the value at the end of the stack
>- peek() to check the value at the end of the stack
>- length() or size() to check the length or size of the stack
>
>:sets:
>- set data structure is like an array except there are no duplicate items.
>- values are not in any particular order.
>- typical use is to check for the presence of an item.

id: 2025-01-15b
source:
tag: #wasm, #emcc
>$ sudo apt install emscripten 
>use the command emcc to compile the C/C++ file
>$ emcc hello_world.c
>it outputs two files. a.out.js and a.out.wasm. add the js file in the html
>file. (ie. <script src="a.out.js"></script>)

id: 2025-01-15a
source:
tag: #rance_sabaku_no_guardian
>similar to golden boy anime but the setting is a fantasy medieval era.

id: 2025-01-14b
source: https://youtu.be/0DO7_4nk0Hg?si=HMEjcy7N6SLB556A
tag: #sterlinig_engine
>In 1816, the 26 year old Robert Sterling invented the sterling engine in 
>Scotland. Recently, Chinese scientist have further develop the sterling 
>engine. Specifically, the thermoacoustic sterling engine. High-pressure helium
>at 15 megapascals serves as the working medium(more than 30 times the
>pressure of a bicycle tire). 

id: 2025-01-14a
source: https://youtu.be/YK7G6l_K6sA?si=2xR3Dubo-DtJb9oF
tag: #heat_transfer
>:conduction: - heat energy is transferred by the collision of molecules or
>other particles.
>:convection: - transfer of heat energy by the physical movement of a fluid -
>which in engineering, can be liquid or a gas.
>:radiation: - is a transfer of heat energy in the form of electromagnetic
>waves - any electromagnetic waves, not just the cancer-causing kind. 
>Reflective surface minimize heat transfer.

id: 2025-01-12a
source:
tag: #artsey.io, #zmk-ardux
>to upload a firmware to nice nano, plug the board to the usb and double click
>on the reset button.

id: 2025-01-10c
source:
tag: #server, #firebase
>- setup a google firebase project
>- install firebase tools for the terminal.($ npm install -g firebase-tools)
>- log into your firebase account. ($ firebase login)
>- ($ firebase init hosting)

id: 2025-01-10b
source:
tag: #mikrotik, #downgrade
>- copy an older version of the firmware to the files.
>- go to device terminal and type /system/package/downgrade

id: 2025-01-10a
source:
tag: #bird_lungs
>bird lung are more effecient than mammals/humans. when they inhale and then
>exhale, it doesn't go through the same way. it goes through another air sac
>before air is released. it's a one way valve unlike humans we're it's a two
>way valve. The air that goes into the lungs go the same pipe to go out. birds
>does this because they can extract 100% of the oxygen in the air and thus 
>delivering more oxygen to the blood stream making them not gasp for air when
>they are flying at high altitude(thin air). there was an incident were a bird
>was injured and its wing was so bad that the bone protruded. when a somebody
>saw this particular bird, he did the most human thing to do and tried to drown
>it. to his surprise, the bird didn't die because the bird's lung is so 
>effecient that they can actually breadth from the protruding bone. like 
>snorkling.

id: 2025-01-09a
source: https://router-network.com/comfast-router-login
tag: #comfast
>default login for comfast
>ip address: 192.168.10.1
>username:   admin
>password:   admin

id: 2025-01-08b
source:
tag: #mikrotik
>at least for the haplite models, when changing the wifi settings, the device
>reboots the wifi module. Don't be surprise if you get disconnected for a 
>minute when using either webfig or winbox.

id: 2025-01-08a
source: https://www.starlink.com/en-ph/support/article/d68ed178-4d54-b486-b7d8-2a6273917632
tag: #starlink, #router, #reset, #gen2
>Power cycle the router 6 times in a row, unplugging and plugging it back every
>time. The router will take a few minutes to reboot.

id: 2025-01-07a
source:
tag: #albatross
>- range widely in the Southern Ocean and the North Pacific.
>- dynamic soaring and slope soaring.
>- eats squids, fish, krill.
>- wingspan of 2.5 - 3.5 meters.
>- by exploiting the energy of the wind, they expense none of their own.

id: 2025-01-06a
source:
tag: #mikrotik
>creating multiple dhcp server
>1. IP/Addresses - add a unique ip address other than the one that is currently used (ie 192.168.89.1/24, 10.0.0.1/24) and assign it to a bridge(ie bridge2 if bridged1 is already used).
>2. IP/IP Pool - add a pool of ip address for this network. Addresses must be in range (ie 192.168.89.20-192.168.89.40).
>3. IP/DHCP Server - create another dhcp server. Address pool should be the newly created pool of ranged addresses from step 2. Interface should be the same bridge used in step 1.
>4. IP/DHCP Server - go to the network tab and add a new network. Address should be 192.168.89.0/24 ang Gateway should be 192.168.89.1 with a Netmask of 24.
id: 2025-01-02c
source:
tag: #geometric_sequence
>- if the initial term is negative and r > 1, the sequence is decreasing.
>- if the initial term is negative and 0 < r < 1, the sequence is increasing.

id: 2025-01-02b
source:
tag: #data_structure, #priority_queue
>Priority Queue - a FIFO data structures that serves elements with highest
>priority first before elements with lower priority.

id: 2025-01-02a
source:
tag: #data_structure, #queue
>Queue - FIFO data structure. First-In First-Out
>A collection design for holding elements prior to processing
>Linear Data Structure
>
>Where are queues useful?
>1. Keyboard buffer
>2. Printer Queue
>3. Used for LinkedList, PriorityQueues, Breadth-first search

id: 2025-01-01d
source:
tag: #javascript, #pop
>pop() - removes the last value in an array.
>Doing a pop() method on an empty array does not give out an error in js.
>You can store the pop() value in an array by assigning it to a variable.
>(ie. let someValue = array1.pop())

id: 2025-01-01c
source:
tag: #data_structure, #stack
>stack - LIFO data structure. Last-in First-out stores objects in a sort of
>"vertical tower" (ie. stack of books, cds, games etc.)
>push() to add to the top
>pop() to remove from the top
>uses of stack?
>1. undo/redo features in text editors
>2. moving back/forward through browser history
>3. backtracking algorithm (maze, file directoris)
>4. calling functions (call stack)

id: 2025-01-01b
source:
tag: #algorithm
>algorithm - a collection of steps to solve a problem
>why learn data structure and algorithms?
>1. You'll write code that is both time and memory effecient.
>2. Commonly asked questions involve DS&A in coding interviews.

id: 2025-01-01a
source:
tag: #data_structure
>data structure - a named location that can be used to store and organize data.
>(ie. family tree, array)

id: 2024-12-31c
source:
tag: #javascript, #closure
>closure - a function defined inside of another function, the inner function
>has access to the variables and scope of the outer function. Allow for
>private variables and state maintenance. Used frequently in JS frameworks:
>React, Vue, Angular

id: 2024-12-31b
source:
tag: #javascript, #callback
>callback - a function that is passed as an argument to another function.
>used to call asynchronous operations:
> 1. Reading a file
> 2. Network request
> 3. Interacting with database
> Hey, when you're done, call this next

id: 2024-12-31a
source:
tag: #javascript, #setTimeout
>setTimeout() - function in javascript that allows you to schedule the execution
>of a function after an amount of time(milliseconds). Times are approximate
>(varies based on the workload of the javascrip runtime env).

id: 2024-12-30b
source:
tag: #javascript, #date
>date objects - object that contain values that represent date and times.
>These date objects can be changed and formatted.

id: 2024-12-30a
source:
tag: #javascript, #sort
>Method used to sort elements of an array in place.
>Sorts elements as strings in lexicographic order, not alphabetical.
>lexicographic - (alphabet + numbers + symbols) as strings.

id: 2024-12-29d
source: https://youtu.be/EvlIWIu8_zk?si=A7DVd0j8ybq4HiIp
tag: #c_programming_2024
>Why do we still use c in 2024?
>C is still heavily use in equipment were hardware and software need to 
>communicate with less overhead(ie. interpreter, os, etc).

id: 2024-12-29c
source: https://youtu.be/Oo7DpNPR-tM?si=rqDSChsBNnwCFvER
tag: #vertical_farming
>vertical farming are failing because of not turning profit due to high cost of
>maintaining the facility(energy cost). Average consumer would not want to buy
>the same lettuce for twice the price of a traditional farming method. But 
>vertical farming is a viable solution for countries that doesn't have a year 
>round climate for farming.(ie. Canada have long winters)

id: 2024-12-29b
source:
tag: #javascript, #destructuring
>destructuring - extract values from arrays and objects, then assign them to 
>variables in a different way
>[] - to perform array destructuring
>{} - to perform object destructuring

id: 2024-12-29a
source:
tag: #javascript, #getter, #setter
>getter - special method that makes a property readable
>setter - special method that makes a property writable
>validate a value when reading/writing a property
>use underscore to indicate a private variable
>(ie. firstName -> this._firstName)

id: 2024-12-28b
source:
tag: #javascript, #super
>super - keyword is used in classes  to call the constructor or access the 
>properties and methods of a parent (superclass)
>this = this object
>super = the parent

id: 2024-12-28a
source:
tag: #javascript, #inheritance
>inheritance - allows a new class to inherit properties and methods from an 
>existing class (parent -> child) helps with code reusability

id: 2024-12-27a
source:
tag: #javascript, #static
>static - keyword that defines properties or methods that belong to a class 
>itself rather than the objects created from that class (class owns anything 
>static, not the objects)

id: 2024-12-26b
source:
tag: #javascript, #class
>class - (ES6 feature) provides a more structured and cleaner way to work 
>with objects compared to traditional constructor function ie. static keyword, 
>encapsulation, inheritance inside of a class you don't need to define the 
>function keyword

id: 2024-12-26a
source:
tag: #javascript, #constructor
>special method for defining the properties and methods of objects

id: 2024-12-25c
source:
tag: #javascript, #this
>this - reference to the object where THIS is used (the object depends on the 
>immediate context)
>person.name = this.name
>note: when you use arrow function in an object, when you call a property 
>(ie. ${this.xxx}) with this. it is referring to the window object of the 
>page. 

id: 2024-12-25b
source:
tag: #javascript, #object
>Object is a collection of related properties and/or methods. Can represent 
>real world objects(people, products, places).
>object = {key: value,
>            function()}

id: 2024-12-25a
source:
tag: #javascript, #arrow_functions
>arrow functions - a concise way to write function expression good for simple 
>function that you use only once (parameters) => some code

id: 2024-12-17d
source:
tag: #javascript, #ternary
>ie.
>function isEven() {
>  return number % 2 === 0 ? true : false;
>}

id: 2024-12-17c
source:
tag: #javascript, #isNaN
>isNaN(num) - a javascript builtin method to check if a variable is a number 
>data.

id: 2024-12-17b
source:
tag: #javascript, #array
>toString() - turns an array of strings(ie names) into one contigous string.
>join() - similar to toString() but with an added parameter of joining them 
>with a character or string between(ie. join(',')adds a coma to every value in 
>index)
>concat() - combined arrays together. several arrays can be added by adding 2 
>or more in the parameters
>splice() - remove a value in an index of array. parameter 1 is the index 
>number and parameter 2 is the number of values to be deleted after the first 
>parameter. copy the original array to be splice to avoid mutation. 
>slice() - takes the value of the original array from and index up to the next 
>but not excluding the current index.
>indexOf() - finds the location of the value in an array. The first from left 
>to right.
>splice() - removes a specified index from and array on the first parameter. 
>second parameter indicates how many indexes to remove starting from the index 
>specified in the first parameter.
>sort() - sorts the array in ascending order. if you want to descend the order 
>you can chain the method by doing sort().reverse() but the drawback with this 
>method is it's slow in terms of effeciency. you can however use a callback 
>function in the sort method. 
>
>sort((a, b) => {
>  if(a === b) return 0;
>  if(a > b) return -1;
>  return 1;
>})
>// 0, a === b, there is no change
>// -1, a sorted before b
>// 1, b sorted before a
>
>indexOf() - starts to search which index of is the first value in the 
>parameter from index 0. returns -1(false) if it didn't find the searched 
>value if there are two or more values that are the same in an array, this 
>method would find the first instance of that searched value. You can however 
>find the next instance of that value by adding a second parameter. 
>indexOf(value1, 1) 1 is the index the method would start searching. if you 
>want to search from the last index instead of index 0, you can use the method 
>lastIndexOf().
>
>findIndex() useful for finding objects in an array.
>
>includes() - checks if a value in an array exist. returns true or false.
>
>some() -  checks if "some" value in an array is true. returns boolean
>every() - checks if "every" value in an array is true. returns boolean
>
>concat() - merging arrays
>let alphanumeric = [...num1, ...num2, ...letters]; - spread operator
>
>slice() - copies an array. if no argument is specified, the method copies the 
>whole array. the first argument indicates the start index to copy and the 
>second argument is the ending index but not including. Which basically means 
>that if you want to copy an index from 2 to 5, the method should look like 
>slice(2, 6)

id: 2024-12-17a
source:
tag: #math
>distributive property - some equations become much easier when we can rewrite 
>them.

id: 2024-12-16a
source:
tag: #keyboard_audio
- bucklespring (https://github.com/zevv/bucklespring)

id: 2024-12-13a
source:
tag: #javascript, #textArea
>appending a textArea by using += (ie. textArea.value += displayedValue)
>to go to a new line, add the "\n" in the value (ie. textArea.value += "\n" + 
>displayedValue)

id: 2024-12-04a
source: https://youtu.be/XA2WjJbmmoM?si=eQucqohOLy6Ekm3W
tag: #vim, #no_plugins

id: 2024-12-02a
source: https://youtu.be/1_gJp2uAjO0?si=f5kmwPWOJt7wj8S5
tag: #quantum_computing, #bloomberg
>- computing with transistors means that a bit can either be 0 or 1s(on/off).
>- quantum bits can be either, both or neither.

id: 2024-12-12a
source: https://youtu.be/YrXw4CmxljA?si=N3blsA2nbhS2URWw
tag: #flywheel, #genrator, #energy
>flywheel is best at smoothing out power fluctuation

