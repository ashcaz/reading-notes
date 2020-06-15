## Heroku Deployment

[Node.js For Beginners](https://howtonode.org/deploy-blog-to-heroku)

setting up a server

```JavaScript
var http = require("http");

http.createServer(function(request, response) {
  response.writeHead(200, {"Content-Type": "text/plain"});
  response.write("It's alive!");
  response.end();
}).listen(3000);
```


[Back to Homepage](https://ashcaz.github.io/reading-notes)