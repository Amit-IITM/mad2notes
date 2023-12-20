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
- "of" iterate over "values"
- if array have holes then JS counts only those indicies which have values.

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
### Var :
### Let :

<hr>

### ⁂ Function :
1. Regular declaration :
2. Named variable :
3. Arrow function :

### ⁂ Call Back function :
A function which can be passed as argument.

### ⁂ special variable "this" : 

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

**CSRF** : Cross Site request Forgery <br>
let's say you login your bank account in one tab and in another tab you open another tab which belongs to hacker. So if Hacker send "withdrawl" request to bank server then bank server will not be able to find difference between sender tab. and Hacker will get your money.<br>
Solution : One time use token

<hr>

