API rate limiter middleware for express 

3 Types of way we can implement it :-
  - using inbuild memory, By default, the built-in memory-store is used.
  - using external memory store like postgres, redis, etc.
  - using a custom external memeory store.

How to run it :-

 - clone the repo switch to master branch
 - npm i
 - node index.js
 - go to http://localhost:3000/api/data in your browser.
 - refresh the page multiple times then you will get Status code 429 (Too many request),
 - wait for 1 minute (configurable to custom value in middleware) then you'll be able to send the request again.
