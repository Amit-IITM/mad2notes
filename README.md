## MAD 2 Notes
### ⁂ Application and it's components
- frontend
- backend
- architrecture
<hr>

**JAM stack** : JavaScript, API, Markup. <br>
              This term is coined by **Mathias Biilmann**.
<hr>

**PWA** : Progressive Web Appliction <br>
          An app which can work in web browser and give same experience as App. It have all features of an App.
<hr>

**SPA** : Single Page App<br>
          If you make some changes in a part of SPA then only that part change, other part remain unaffected.
<hr>

**Asynchronycity** : Multiple task at the same time without being in synchronizing to each other. No direct time relationship between them.
<br>
**Ajax** : Asynchronous JavaScript And XML
<hr>

**ECMA** : European Computer Manufacturers Association
<hr>

**Polyfills** : Libraries which use new functionalities in old browsers.
<hr>

**Linter** : A tool which go to source code and gives us idea about improving our code.
<hr>

**DOM** : Document Object Model<br>
Structure of document on browser, You can directly change what you are seeing.
<hr>

**Array** : Collection of objects of any data type. We can have array of single data type or we can have different data types. we can also have holes in array.

<hr>

**Destructuring** : spliting an array into multiple variables.
<hr>

**Hoisting** : It appears to move "Declaration" at the top of your code before execution.
```
 x = 5
var x
```
I declared var x after x = 5. logically it seems backward but it's fine in JS with hoisting. <br>  <br>
It happenes with "function" and "var" but not with "const" and "let".
  - with function, hoisting gives "value".
  - with var, hoisting gives "Undefined".
<hr>

**AMD** : Asynchronous module Definition
<hr>

**npm** : Node Package Manager
  Command line interface of js; mainly used for backend code and testing.
<hr>

**JSON** : Java Script Object Notation <br>
Relly good if we want to transfer an object from one place to another. Json is frozen, no further developement.
  - JSON.stringify() : takes one object and converts it into string.
  - JSON.parse() : String to object
<hr>

- Default port number of Flask application is **5000**.
- JS engine generally use **UTF-16** encoding.
- ```===``` use in avoiding coercion in JS. because JS is a tolrent language.
- **Templates** Starts with `backward quotes.   ${ variable name }
- ```
  for (let x = 0; x < 5; x++) {
      console.log(x);
      }
  ```
  we can't use const here or for loop will not run.
- **Await** function for time lag.
- **inner HTML** : modifying HTML through JavaScript.
- **Literals** : they represents values in JS. These are fixed values.
   - True is not a valit litral in JS.
- ```
  let x = 200
  console.log(x)    => 200
  console.log(x.value)      =>  undefined
  ```
- String is not a collection. Array, Map (very much like dictionary), set are collections.
- "in" iterates over "indicies".
  ``` for i in ['a','b','c'] => 0,1,2```
- "of" iterate over "values"
  ```for i of ['a','b','c'] => a,b,c```
- if array have holes then JS counts only those indicies which have values.
- ```
  True * True = 1
  False * False = 0
  True * False = 0
  ```
- when we define a function inside { }, then always use "return".
- use **set time out**  with **set interval**.
- **length** method is defined only for array, not for other objects.

<hr>

### ⁂ Applets :
- written in Java, embeded in HTML
- way of adding applets in HTML
    1. ```<applet code = "....."></applet>```
    2.  ```<applet = "....."></applet>```
- works in web browser directly.
- Then need of new language => **JavaScript**
- JavaScript was **ECMA-Script** officially.
    1. JS can be use for DOM manipulation.
    2. Client side scripting language, less load on server
    3. use in asynchronous processing
    4. use in event loop.
- **ES6 in 2015** : Significant changes
- It was designed to ensure the interportability of webpages across the browsers.
- Java Script was not running into many old browsers so we could use
    1. Package browser along with Applictions
    2. Use Polyfills
    3. Use Compilers , which can convert new JS into older version.

<hr>

### ⁂ Data Types in JS :
1. Primitive : Built into the language
     1. undefined
     2. null
     3. boolean
     4. number
     5. string
     6. Big int
     7. symbol
3. Objects : Multiple things put together
4. Functions : Can be handled like objects

<hr>

### ⁂ Let, Var, Const :

|x|Scope|Redeclare|Reassign|Hoisted|Bind this|
|---|---|---|---|---|---|
|var| Global | Yes | Yes | Yes | Yes|
|let| Block | No | Yes | No | No |
|const| Block | No | No | No | No |

### Const :
We need to assign value to const at the moment of defining. Can't change it's value throughout JS code.
### Var :
Globally scoped, you can change it from anywhere.
<br>
Even if you change the value of Var inside block, it'll affect it globally.
### Let :
here if you change value inside block then that value will changed only for block. block ki baat block me, bahar ki bahar.

<hr>

### ⁂ Function :
1. Regular declaration :
2. Named variable :
3. Arrow function :

### ⁂ Call Back function :
A function which can be passed as argument.

### ⁂ special variable "this" : 
This keyword refers to the current object in a method or constructor. when "this" is inside a function it owns the value of that function. When it's outside a function then it owns the global value.
<br> If "this" is not set by a call then it'll have the value of global object.
<br> **Arrow function** doesn't pick the value of "THIS" from it's own block. it picked value of THIS from immediate surrounding. 

<hr>

### ⁂ Prototype and heritance :
In JS we can define one object "a" and other object "b". and make b as prototype of a. So b will inherit properties of parent object a. this is called **Prototype based inheritance**.<br>
**Single Inheritance Track**, we can have only direct parent-children relationship.

<hr>

### ⁂ Stack frame - Call Stack - event Loop :
Stack of all function provided. First in - Last out. <br>
if 4 function at once then stack will have 4 functions. now if we provided 1 more function then it'll go into queue. and queue works on first in - first out. This is called **Task Queue**.<br>
Taking task out of queue and put it onto stack and start executing till call stack become empty. this process is called **Event Loop**.<br>
once a task make to call stack it must be completed before next task is evoked.

<hr>

⁂
```
let a = [1,2,3,4,5]
console.log(object.values(a)) = [1,2,3,4,5]
console.log(object.keys(a)) = ['0','1','2','3','4']
console.log(object.entries(a)) = [['0',1]['1',2],...,['4',5]]
```

<hr>

### ⁂ UI and UX :
**UI** : User Interface. related to the aesthetics of the application.
**UX** : User experience. How user interact with the application.
<br>
**Requirements** :
- all computations and logic must be in backend.
- No data storeage in frontend, only representation of results, which are requested.
- must suport stateless nature of HTTP.
<br>
**Desirable aspectrs** :
  - Aesthetically pleasing : not ugly
  - Responsive : No lag, immediate response
  - Adaptive : Different size screen adaptiveness

<hr>

### ⁂ Programming style :
**Imperative** :
If you want some result then, You need to formulize all steps. Steps Oriented
<br>
**Declarative** :
Focus on final result, steps will follow. Result oriented

<hr>

### ⁂ State :
Memory of the system
<br>
**System State** : Describes entire system.
**Application state** : Syatem as seen on user/session. It includes interactivity and session management. everything which is present in the screen when app is running.
**UI state** (Ephimereal state) : very short lasting. Part of application which actually interects with user.

<hr>

### ⁂ Persistant and Non-Persistant data :
Persistent data lasts longer than application. It stays available even you fully closed the application and restart the application. ex. System state or Application state.
<br>
Non-Persistant data very voletile data, disappeared as soon as you close your application. ex. Epemeral state.
<br> <br>
**Local Storage** is a client side storage, data will persist even if app refreshes. or browser restarts.
  - Local Storage doesn't have remove() method.
<br>


<hr>

### ⁂ Vue
Core idea behind Vue is **Declarative Rendring**. main focus on what need to be shown.
<br>
**Reactivity** : Automatically update certain parts of display in response of change-in-data.

<hr>

**IIFE** : Immediately Invoked Function Expression<br>
this function executed immediately as soon as we define it.<br>
it's structure is not like ```function(){something()}```
but like ```(function(){something()})()```

<hr>

**Higher Order Functions** : A function that accepts functions as parameters and/or returns a function.

<hr>

### ⁂ Life cycle hooks / Component Life cycle hooks
4 different phases through which component goes through in a Vue application.<br>
1. Creation : Before create, created
2. mounting : Before mount, mounted
3. updating : before update, updated
4. Unmounting : before unmounted, unmounted
<br>
5 more methods : activated, deactivated, error captured, render tracked, render triggered.
<br><br>
```
parent before created => created => before mount
child before created => created => beofre mounted => mounted
parent mounted => before update
child before unmounted => unmounted
parent updated
```

<hr>

### ⁂ Async / Await in Java Script :
A simple function, it gives you whatever you enters.<br>
Just add "async" before function and it'll give you promise. it'll not give you exact output but promise.

### ⁂ Promise :
It is an object that will produce a single value some time in future. <br>
Three stages :
- pending
- fullfilled
- rejected
<br>
Async functions always returns a promise.

<hr>

**Local storage**:
- it's client side storage
- each time app refreshes, the data will still persist
- only string type data is stored in local storage

<hr>

### ⁂ Threaded Server :
generally servers don't take more requests when they work on a request. They are caled **Blocking server**.<br>
But Threaded server accept incoming request and start working on it. if another request comes then go and listen to that request too.

**Concurrent** : Doing one task and then jumping to another. very fast jumping. so it seems like that both tasks are handled at the same time. but no.
<br>
**Parallelism** : We have hardware to deal with this situation. we can use 2 or more CPU to handle different tasks.

<hr>

### ⁂ Redis :
Redis is a tool to design Database. It is a "No SQL" database. No table or document required. All data saved in Key - value pairs in JSON format. Redis runs on our working memory **RAM**. very fast but voletile. It's not persistant database but runs in cache memory. Redis makes things faster, 10x to 50x .<br>
<br>
**6379** is the permanent **port** number for Redis.<br>
**quit** : exit<br>
**set** : Set a key and it's value<br>
**get** : get that already seted key's value<br>
**del** : delete a specific key<br>
**exists** : check if any key exists<br>
**Key \*** : gives us all keys at once.<br>
**Flushall** : removes all keys<br>
**clear** : to clear screen<br>
**ttl** : time to live<br>
  - generally output is -1, which shows this key will live forever.
  - after giving **expire key time**, ttl gives remaining time
  - and -2 means, key is already gone.

<hr>

### ⁂ Webhook
It's a code which triggers when desired thing happens

<hr>

**PII** : Personally Identifiable Information <br>
### Sensitive Information : 
  - **Direct** : this information is given by user, and user knows about it.
  - **Indirect** : this is related information, kind of Meta Data. which is not given by user directly.
<br>

**GDPR** : General Data Protection Regulation <br>
required in EU for any business, cause of "cookies notice".
<br>
**HIPAA** : Health Insurance Portability and Accountability Act <br>
US specific, protect data of patients and policy holder.

<hr>

### ⁂ Front End Security :
1. **Site interaction** : how user interact with sites. <br>
  - Static site : No info of user
  - Form based site : user fill the form and this is the only info which we can get
  - Dynamic site with JS : Complex site and we get lots of collected data
2. **Resources** :
    - cookie based site tracking
    - **CDN** traking (Content Delivery Network)
3. **Browser Exploits** : Malware, spyware, login data leakes, cross tab etc

**Cross Site Scripting** : (XSS) <br>
add some exploit in a website and when someone clicked on that link, it'll transfer all data to you ( mostly sessin cookies). and you can use this data to log in. <br>

**CSRF** : Cross Site request Forgery <br>
let's say you login your bank account in one tab and in another tab you open another tab which belongs to hacker. So if Hacker send "withdrawl" request to bank server then bank server will not be able to find difference between sender tab. and Hacker will get your money.<br>
Solution : One time use token

<hr>

