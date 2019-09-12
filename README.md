# WebDev - WebDev re notes...

0) Dev environment - Glitch.com
    - https://anidiots.guide/other-guides/hosting-on-glitch
    - https://flaviocopes.com/glitch/
    - https://blog.bitsrc.io/introduction-to-glitch-for-node-js-apps-in-the-cloud-cd263de5683f

1) http basics - https://www.youtube.com/watch?v=iYM2zFP3Zn0
    - outline - destination (protocol, address, port), methods, headers
    - request / response cycles
    - methods - get, post, put, delete
    - headers - general, request, response
    - body
    - status codes - 1xx, 2xx, 3xx, 4xx, 5xx
    - http 1.1 vs http 2
    - use postman tool (or chrome extension) for testing get, post, put, delete methods for diff requests/responses with Node/Express

    Tentative Dev Stack as of now? - 
    - Current - node (on Glitch), w3.css/w3.js - express - sqlite
    - future? - w3.css/jquery - deno - ??????? - sqlite

2) Decoupling Your HTML, CSS, and JavaScript - https://philipwalton.com/articles/decoupling-html-css-and-javascript/
    - Classes should be the glue that connects your HTML, CSS, and JavaScript together. 
        - Don’t use the same class for both style and behavior.
           - use a prefix js-* for all JavaScript hooks
           - using the prefix is-* for all the styling hooks
        - Style components based on what they are, not where they are. Classes Are Your Contract.
           Instead of a CSS file defining complex selectors,
           simply define the look of a visual component via a single class. The HTML may then choose to use that class or not use it.
           Instead of using JavaScript for complex DOM traversal functions,
           simply listen for the user’s interaction with elements that contain the agreed-upon class names
        - Favor explicit component and behavior classes over complex CSS selectors in both CSS and JavaScript.
        - Differentiate state styles from default styles.

4) Unobstrusive JS pattern
	- In html, Structure and content elements which will have the input or output are tagged by id / class
	- In script at the start, all id / class tags are queried and mapped to variables (declared as const) using queryselector
	- Subsequently, all code uses the variables alone to manipulate the elements
	- Sample
	. var elementClassOrId = document.querySelector('elementClassOrId');
	. function eventHandlerFunction1() {
	. //event handler code
	. }
	elementClassOrId.onclick = eventHandlerFunction1;

3) Avoid frameworks 
    Why avoid frameworks as much as possible - https://dev.to/gypsydave5/why-you-shouldnt-use-a-web-framework-3g24
    
    A Framework Author's Case Against Frameworks - https://www.youtube.com/watch?v=k7n2xnOiWI8

4) Use Chrome developer tools as IDE/Debugger
    https://developers.google.com/web/tools/chrome-devtools/?utm_source=dcc&utm_medium=redirect&utm_campaign=2016q3
    
    https://gregrickaby.com/2013/07/turn-chrome-developer-tools-into-an-ide/
    
    go to chrome://flags/, and enable "Developer Tools experiments"
    press ctrl + shift + p in chrome developer mode and enable reverse mode

    OR
    
    Use Microsoft Visual Code editor

5) HTML Page template (to be uploaded)

6) W3.CSS - pure css framework
   - explore other pure css frameworks or moduler frameworks... (bulma, siimple etc)
   - check grid systems, css components application for layouts

7) W3.JS - lightweight JS library
   - explore pure JS libraries like MithrilJS etc

8) A Very Simple Demonstration of Node.js / Express and SQLite - 
   https://stealthistech.blogspot.com/2013/09/a-very-simple-demonstration-of.html

   Mozilla ExpressJS tutorial
   https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs

   Understanding Express.js
   http://evanhahn.com/understanding-express/
   
9) 2 way data binding in pure JS
    https://github.com/janubande/2WayDataBindJS

10) Web server - NodeJS or Deno?
    Original slides from Ryan Dahl's NodeJs intro talk -
    https://www.slideshare.net/AartiParikh/original-slides-from-ryan-dahls-nodejs-intro-talk

    Ryan Dahl's recent presentation on Deno features
    https://www.youtube.com/watch?v=z6JRlx5NC9E
    
11) Debugging Node.js with Chrome DevTools
    https://medium.com/@paul_irish/debugging-node-js-nightlies-with-chrome-devtools-7c4a1b95ae27
    Open chrome://inspect/#devices and go to "Open dedicated DevTools for Node"

    Understand difference in debugging client-side and server side javascript

    ??? check above to debug Deno...

12) Tools to Automate Restarting Node.js Server After Code Changes - Forever or Nodemon module -> cmd -: foreever -w <script>
https://strongloop.com/strongblog/comparison-tools-to-automate-restarting-node-js-server-after-code-changes-forever-nodemon-nodesupervisor-nodedev/

??? check above to debug Deno...

13) Server side rendering - 
    ExpressJS
    OR
    Fastify https://blog.logrocket.com/forget-express-js-opt-for-these-alternatives-instead/
    OR
    UWebSockets - https://levelup.gitconnected.com/will-node-js-forever-be-the-sluggish-golang-f632130e5c7a
    OR its express like wrapper - nanoexpress - https://github.com/dalisoft/nanoexpress

    ??? check above to debug Deno...
    
    SSR capabilites to learn -
    - routing
    - middleware
    - template engine (can one use say Vue/Nuxt.js instead of Jade/Pug as template engine)
    - DB interface
    - enable SSL/HTTPS
    - auth - stateful (session based with cookie) 
    - auth - stateless (token based with Oauth, jwt...)

14) Auth - session or token based? 
    - https://stormpath.com/blog/choosing-nodejs-authentication-strategy
    
    - Use Passport for now
    
    - Later, expore aspects post authorisation like logins, persistence, sessions etc... -> using "Authum"
    
15) Object request mapper - 
    use query builder(Knex.JS)
    OR
    raw DB driver? - DB - Sqlite module (http://www.sqlitetutorial.net/sqlite-nodejs/)

    https://blog.logrocket.com/why-you-should-avoid-orms-with-examples-in-node-js-e0baab73fa5/ 

    ??? check above to debug Deno...

16) sqlite or nedb

 ______________________________________________________________________________________________________________________ 
 
For later exploration...

16) eslint - http://www.codingfordummies.org/detect-errors-in-your-javascript-code-with-eslint/

17) Jvascript code snippets - 
    - vscode feature https://code.visualstudio.com/docs/editor/userdefinedsnippets
    - how to use https://www.freecodecamp.org/news/the-most-powerful-tool-to-boost-your-coding-productivity-2dc80e0eff00/

    - snippet generator - https://snippet-generator.app
    
    - w3school snippets https://www.w3schools.com/howto/default.asp

18) refactoring - https://www.youtube.com/watch?v=6wDoopbtEqk

https://github.com/cmstead/js-refactor

Misc -:
Web Developer Roadmap - Ref: https://github.com/kamranahmedse/developer-roadmap
