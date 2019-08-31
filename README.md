# WebDev
WebDev re documents

http basics - https://www.youtube.com/watch?v=iYM2zFP3Zn0
- request / response cycles,
- methods - get, post, put, delete,
- headers - general, request, response,
- body,
- status codes - x,
- http 1.1 vs http 2,
- use postman tool (chrome extension) for testing get, post, put, delete methods for diff requests/responses with Node/Express

Tentative Stack as of now? - 
- Current - w3.css/w3.js - node - express - sqlite
- future? - w3.css/jquery - deno - ??????? - sqlite

0) Avoid frameworks 
    Why avoid frameworks as much as possible - https://dev.to/gypsydave5/why-you-shouldnt-use-a-web-framework-3g24
    
    A Framework Author's Case Against Frameworks - https://www.youtube.com/watch?v=k7n2xnOiWI8

1) Use Chrome developer tools as IDE/Debugger
    https://developers.google.com/web/tools/chrome-devtools/?utm_source=dcc&utm_medium=redirect&utm_campaign=2016q3
    
    https://gregrickaby.com/2013/07/turn-chrome-developer-tools-into-an-ide/
    
    go to chrome://flags/, and enable "Developer Tools experiments"
    press ctrl + shift + p in chrome developer mode and enable reverse mode

    OR
    
    Use Microsoft Visual Code editor

2) HTML Page template (to be uploaded)

3) W3.CSS - pure css framework
   - explore other pure css frameworks or moduler frameworks...
   - check grid systems, css components application for layouts

4) W3.JS - lightweight JS library

5) A Very Simple Demonstration of Node.js / Express and SQLite - 
   https://stealthistech.blogspot.com/2013/09/a-very-simple-demonstration-of.html

   Mozilla ExpressJS tutorial
   https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs

   Understanding Express.js
   http://evanhahn.com/understanding-express/
   
6) 2 way data binding in pure JS
    https://github.com/janubande/2WayDataBindJS

7) Web server - NodeJS or Deno?
    Original slides from Ryan Dahl's NodeJs intro talk -
    https://www.slideshare.net/AartiParikh/original-slides-from-ryan-dahls-nodejs-intro-talk

    Ryan Dahl's recent presentation on Deno features
    https://www.youtube.com/watch?v=z6JRlx5NC9E
    
8) Debugging Node.js with Chrome DevTools
    https://medium.com/@paul_irish/debugging-node-js-nightlies-with-chrome-devtools-7c4a1b95ae27

    Open chrome://inspect/#devices and go to "Open dedicated DevTools for Node"

    ??? check above to debug Deno...

9) Tools to Automate Restarting Node.js Server After Code Changes - Forever or Nodemon module -> cmd -: foreever -w <script>
https://strongloop.com/strongblog/comparison-tools-to-automate-restarting-node-js-server-after-code-changes-forever-nodemon-nodesupervisor-nodedev/

??? check above to debug Deno...

10) Server side rendering - 
    ExpressJS
    OR
    Fastify https://blog.logrocket.com/forget-express-js-opt-for-these-alternatives-instead/
    OR
    UWebSockets - https://levelup.gitconnected.com/will-node-js-forever-be-the-sluggish-golang-f632130e5c7a
    OR its express like wrapper - nanoexpress - https://github.com/dalisoft/nanoexpress

    ??? check above to debug Deno...

11) Object request mapper - 
    use query builder(Knex.JS)
    OR
    raw DB driver? - DB - Sqlite module (http://www.sqlitetutorial.net/sqlite-nodejs/)

    https://blog.logrocket.com/why-you-should-avoid-orms-with-examples-in-node-js-e0baab73fa5/ 

    ??? check above to debug Deno...

 ______________________________________________________________________________________________________________________ 
 
For later exploration...

12) refactoring - https://www.youtube.com/watch?v=6wDoopbtEqk

https://github.com/cmstead/js-refactor

Misc -:
Web Developer Roadmap - Ref: https://github.com/kamranahmedse/developer-roadmap
