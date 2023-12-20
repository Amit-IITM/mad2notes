## MAD 2 Notes
### ⁂ Application and it's components
- frontend
- backend
- architrecture

### ⁂ Some Acronyms and defenitions

**JAM stack** : JavaScript, API, Markup. <br>
              This term is coined by **Mathias Biilmann**.

**PWA** : Progressive Web Appliction <br>
          An app which can work in web browser and give same experience as App. It have all features of an App.

**SPA** : Single Page App<br>
          If you make some changes in a part of SPA then only that part change, other part remain unaffected.

**Ajax** : Asynchronous JavaScript And XML

**ECMA** : European Computer Manufacturers Association

**Polyfills** : Libraries which use new functionalities in old browsers.

**Linter** : A tool which go to source code and gives us idea about improving our code.

**DOM** : Document Object Model<br>
Structure of document on browser, You can directly change what you are seeing.

### ⁂ Some facts
- Default port number of Flask application is **5000**.
- JS engine generally use **UTF-16** encoding.
- ```===``` use in avoiding coercion in JS.

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

### ⁂ Let, Var, Const :
|x|Scope|Redeclare|Reassign|Hoisted|Bind this|
|---|---|---|---|---|---|
