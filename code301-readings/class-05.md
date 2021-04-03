# deploy-blog-to-heroku-

## Node JS

Node.js is an open source, cross-platform runtime environment, which allows you to build server-side and networking applications. It's written in JavaScript and can be run within the Node.js runtime on any platform.

## steps

1. Create a server

we will create a file called server.js with the following code:

```
var http = require("http");

http.createServer(function(request, response) {
  response.writeHead(200, {"Content-Type": "text/plain"});
  response.write("It's alive!");
  response.end();
}).listen(3000);
```

to make sure that our server is working we should type in the terminal

```
node server.js
```

2. Make it worldwide

- Works fine. But it works locally. WWW is for "World Wide Web" and we will turn your local server into a world wide server.

- We'll use Heroku cloud application platform for this. Heroku is a cloud platform as a service

- It allows you to deploy your web server, so everyone could see how awesome you are as a web developer.

## how to deploy it actually ?

- fitse step is login in the system from your computer

this a berif introduction toyou can continue from here to more [details](https://https://howtonode.org/deploy-blog-to-heroku)
