<h1>Week #12 challenges</h1>
<h1>Week challenges (Monday) 💻</h1>
<h2>"Time to catch up ⏱️ or play with the React project</h2>
<b></b>
<h1>Week Challenges (Tuesday) 🐣</h1>
<h2>Node.JS Core Understanding</h2>
<b>1. What is Node.JS?<br>
Node.js is a tool that allows you to use JavaScript outside of web browsers. It lets you run JavaScript on the server-side, which means you can use it to build things like web servers and other network applications.
</b>
<br><br><b>
What is NPM?<br>
NPM (Node Package Manager) is a tool that comes with Node.js. It helps you manage and use other people's JavaScript code in your own projects. You can easily install, update, and share code libraries (packages) using NPM.
</b>
<br><br><b>
2. What problem does Node.JS solve (Is there any problem that can be solved with Node.JS 🤔)?<br>
  Node.js helps solve the problem of handling lots of connections at the same time and dealing with tasks that need a lot of input/output (I/O). Traditional methods of handling connections can be slow and use up a lot of memory. Node.js uses a special way of working that allows it to handle many connections efficiently and perform tasks quickly.
</b>

<br><br><b>
3. What is the V8 Javascript Engine?<br>
The V8 JavaScript engine is a program that reads and runs JavaScript code. It was created by Google and is used by Node.js. The engine takes JavaScript code and translates it into instructions that the computer can understand and execute. It's known for being very fast and efficient.
</b>

<br><br><b>
4. Is Node.JS really necessary in the Development ecosystem?<br>
Node.js is not absolutely necessary, but it offers some unique benefits. It's especially useful for building applications that need to handle many connections at once or perform a lot of I/O tasks. It also allows developers to use the same language (JavaScript) for both the front-end and back-end of their applications, which can make development faster and more efficient.
</b>

<br><br><b>
Why not use PHP or Golang?<br>
PHP and Golang are also good options for server-side development, and the choice depends on the specific project and requirements. PHP is well-established and has a large community and many resources available. Golang is known for its performance and built-in concurrency features. The choice between Node.js, PHP, or Golang depends on factors like the project's needs, the development team's familiarity with the language, and performance considerations.
</b>

<br><br><b>
5. What is the difference between Node.JS and any other browser?<br>
Node.js and web browsers are different because they have different purposes and environments for running JavaScript. Node.js runs JavaScript on the server-side and is used for building server applications. It provides tools for working with files, networks, and system operations. Web browsers, on the other hand, run JavaScript on the client-side and are used for displaying and interacting with web pages. They have features for manipulating web page elements, handling user interactions, and working with browser-specific functionalities.
</b>

<br><br><b>
Are Node.JS and a browser the same?<br>
No, Node.js and a web browser are not the same. Node.js is a tool for running JavaScript on the server-side, while a web browser is a program that displays and interacts with web pages. They have different purposes and capabilities, even though they both can run JavaScript.
</b>

<br><br><b>
6. NVM is a tool that allows Node.js developers to manage and switch between multiple versions of Node.js on the same machine.
</b>

<h2>Node.JS Module System Core Understanding Learning Exercise 🧠</h2>
<b>Now that you have a clearer concept about what Node.JS is, it's time to practice with one of its most important concepts: The Module System.
<br><br>
Please answer the following questions with your own words:</b><br><br>
<p>1. What is a JavaScript Module?<br>
A JavaScript module is a small piece of code that does a specific task. It's like a little package that contains functions, variables, or data that can be reused in different parts of a program. Modules help keep code organized and make it easier to work on large projects.</p>

<p>2. Why are JavaScript Modules necessary?<br>
JavaScript modules are necessary because they make code more organized and reusable. Instead of having one big file with all the code, modules allow us to break it down into smaller, self-contained pieces. This makes it easier to understand, maintain, and collaborate on the code. Modules also help prevent conflicts between different parts of the code and make it easier to manage dependencies.</p>

<p>3. What module standards are available in Node.JS?
In Node.js, there are two module standards:<br>
CommonJS: This is the older standard that Node.js originally used. It uses require() to import modules and module.exports or exports to export functionality.
<br>ESModules (ECMAScript Modules): This is the newer standard based on the ECMAScript specification. It uses import and export keywords to import and export modules.</p>

<p>
4.What are the differences between ESModules and CommonJS modules?<br><br>
The main difference between CommonJS and ES modules is the file structure. With CommonJS, all of the dependencies for a project are stored in one file called node_modules/. With ES modules, each dependency is stored in its files.
  
</p>
<p>5. Which types of modules exist in Node.JS?<br>
-Core Modules<br>
-Third-Party Modules<br>
-Local Modules<br>
</p>
<h2>Node.JS Hello World - Practice</h2>

<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/e2a211ac-327f-4bad-9e5c-9c5d9fbe9df4">

<p>
  0. Why do we run the npm init command and not node init to create a new Node.JS project?<br>
  We run the npm init command instead of node init because npm (Node Package Manager) is a tool that helps manage JavaScript packages and dependencies. It provides commands to initialize and manage projects, while node is the command used to run JavaScript code.<br><br>
  1. When you entered the npm init command and answered the questions you saw in the terminal, a new file called packacke.json was generated.<br>
  The package.json file acts as a manifest or configuration file for a Node.js project. It contains important information about the project, such as its name, version,   dependencies, and more. It serves as a central place to document and manage project-related details.<br></br>
  -What does this file do?<br>
  The package.json file in a Node.js project serves as a manifest or configuration file that contains important information and settings related to the project.<br><br>
  -Why is this file generated?<br>
  The package.json file is generated in a Node.js project for several reasons: Dependency Management, Package Publishing, Script Definitions.
</p>
<h2>Node.JS Module System Practice 💻</h2>


~~~javascript

// operations.js
function sum(a, b) {
  return a + b;
}

function subtract(a, b) {
  return a - b;
}

module.exports = {
  sum,
  subtract,
};

~~~

~~~javascript

// main.js
const { sum, subtract } = require("./operations");

console.log(sum(5, 3)); 
console.log(subtract(10, 4)); 


~~~
<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/21d0256f-d103-4682-b53f-399310373540">

<h1>Week challenges (Thursday) 💻🐔</h1>
<h2>1. Express.JS Core Understanding Learning Exercise 🧠</h2>

~~~javascript

const express = require("express");
const app = express();
const port = 3000;

app.get("/", (req, res) => {
  res.send("Hello World!");
});

app.listen(port, () => {
  console.log(`Example app listening on port ${port}`);
});

~~~
<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/ae097200-a9df-4ac1-8399-3f7c1b1f1c00">
<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/f83782cd-1dfb-4daf-b6fb-943211156884">
<h2>2. Forrest Gump Ping-Pong API 🏓</h2>


~~~javascript

const express = require("express");
const app = express();
const port = 3000;

app.get("/api/buba-gump", (req, res) => {
  const playerMove = req.query.move;

  if (playerMove === "ping") {
    res.json({ message: "pong" });
  } else if (playerMove === "pong") {
    res.json({ message: "ping" });
  } else {
    res.status(400).json({ error: "Invalid move" });
  }
});


app.listen(port, () => {
  console.log(`Server is running on port ${port}`);
});


~~~
<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/7c19ad5e-1ff0-44fd-a646-4c5297d0471c">

<h2>Delayed Response API ⏳ Practice 💻</h2>

~~~javascript

const express = require("express");
const app = express();
const port = 3000;

app.get("/api/delay/:time", (req, res) => {
  const delay = parseInt(req.params.time, 10) || 1000;

  setTimeout(() => {
    res.send("Delayed response!");
  }, delay);
});

app.listen(port, () => {
  console.log(`Server is running on port ${port}`);
});

~~~
<img src="https://github.com/drewbydiego/core-code-from-scratch-readme/assets/76753050/f59eea0d-631a-461c-810a-3855a63c7049">
