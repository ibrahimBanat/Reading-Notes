# what is node js ?

There are plenty of definitions to be found online. Let’s take a look at a couple of the more popular ones. `This is what the project’s home page has to say:`

> Node.js® is a JavaScript runtime built on Chrome’s V8 JavaScript engine.

And this is what `Stack Overflow has to offer`:

> Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library.

## V8 JavaScript Engine

`The V8 engine` is the open-source JavaScript engine that runs in Google Chrome and other Chromium-based web browsers, it was designed with performance in mind and is responsible for compiling JavaScript directly to native machine code that your computer can execute.

This means that Node.js is a program we can use to execute JavaScript on our computers. In other words, it’s a JavaScript runtime.

## “Hello, World!” the Node.js Way

- first of all check out the node version by hitting `node -v` in the command line. you should be ending up with something like `v12.14.1`

- Next, create a new file `hello.js` and copy in the following code:

```
console.log("Hello, World!");
```

This uses `Node’s built-in` console module to display a message in a terminal window. To run the example, enter the following command:

```
node hello.js
```

## npm, the JavaScript Package Manager

Node comes bundled with a package manager called npm. To check which version you have installed on your system, type npm -v

## What Is Node.js Used For?

Now that we know what Node and npm are and how to install them, we can turn our attention to the first of their common uses: installing (via npm) and running (via Node) various build tools — designed to automate the process of developing a modern JavaScript application.

These build tools come in all shapes and sizes, and you won’t get far in a modern JavaScript landscape without bumping into them. They can be used for anything from bundling your JavaScript files and dependencies into static assets, to running tests, or automatic code linting and style checking.
