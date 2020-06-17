# Node, Express and APIs

[An Introduction to Node JS](https://www.sitepoint.com/an-introduction-to-node-js/)


## What is Node and When Should I Use it?

**What is Node.js**


Node.js is a program we can use to execute JavaScript on our computers. In other words, it’s a JavaScript runtime

**What is Node.js Used For?**


Node.js lets us run JavaScript on the Server

**Node.js Executin Model**


Node.js, however, is single-threaded. It’s also event-driven, which means that everything that happens in Node is in reaction to an event. For example, when a new request comes in (one kind of event) the server will start processing it. If it then encounters a blocking I/O operation, instead of waiting for this to complete, it will register a callback before continuing to process the next event. When the I/O operation has finished (another kind of event), the server will execute the callback and continue working on the original request.


***What Kind of Apps is Node.js Suited For?**

- Node is particularly suited to building applications that require some form of real-time interaction or collaboration
  - chat sites
  - sites that rewuire live editing
  - good fit for building APIs
  - sites involving data streaming

**What Are the Advantages of Node.js?**

- Speed and Scalability
- You can do everything is  the same lanugage when building a back end a nd a front end of a site. which can make you more roductive as a develeoper.
- It speak JSON
- JaveScript is ubiquitous

**Other Uses of Node**

- As a scripting laguage
- It can be used to write your own command line tool
- Create cross platform desktop apps


[Back to Homepage](https://ashcaz.github.io/reading-notes)