<div class="text-white bg-blue mb-2"><h1>Introduction to JavaScript</h1></div>
Welcome to Complete JavaScript Guide, A that starts from basic like DOM Structure, declaring variables, learning about functions, declarations, classes most modern things like promises async JavaScript, spread operators, and most importantly DOM manipulation and building projects with it. Throughout the course, we will try turning out the toughest topics in the easiest possible way, so that programming becomes fun and engaging. We will wrap up all the concepts related to JavaScript in these modules

JavaScript is a full-fledged dynamic programming language that can add interactivity to a website. It was invented by Brendan Eich (co-founder of the Mozilla project), the Mozilla Foundation, and the Mozilla Corporation. JavaScript is versatile and beginner-friendly. With more experience, you'll be able to create games, animated 2D and 3D graphics, comprehensive database-driven apps, and much more. JavaScript itself is relatively compact, yet very flexible. Developers have written a variety of tools on top of the core JavaScript language, unlocking a vast amount of functionality with minimum effort.

JavaScript has developed a lot and hence there’s a need for the guide which is not a band-aid guide over the existing ones but a completely full-furnished fresh guide, that teaches you a lot about JavaScript, directly by writing the code as well as by understanding some of the behind the scene concepts of JavaScript. How it works??, How the Global Execution context works? How ‘this’ keyword works?? How the spread operator and rest operator are different from each other and a lot more topics like that.
Learning all these Topics about JavaScript is necessary, it’s important but what’s more important is learning with fun, a content that is engaging that you enjoy the whole lot learning process and that’s why we have included projects to give more emphasis on project-based learning. The projects are DOM based so that the process of learning doesn’t seem boring and practice and we learn where to implement JavaScript.

So, we will initially start with installing the tools and writing our very first code. We will do the #classic “Hello World!!” and after that, we will move on understanding about variables, conditionals, and loops, though the guide is not structured in a bookish manner. We have modified the guide structure to make it more fun-learning and we can understand every topic int the easiest manner. So, the guide structure is a bit different and we have included challenges as well to get the best out of it so that you can get to know you have got the concept or not like we have learned it here and I am implementing it here.

Pre-requisites: Zero (0) Seriously, you can begin with no knowledge. You don’t need to have any prior knowledge of other languages like C, C++, Python, Java, etc anything like that you can directly learn it as a very first Language. (Warning: HTML and CSS are not Programming Languages 😊) And we hope it would be whole lot fun learning JavaScript.
Just 10 minutes of daily walk through each module, you can be a JavaScript expert. There will be a whole lot of knowledge of insight behind the scenes of JavaScript that you are goanna thoroughly enjoy. One request from our side if you find anyone stuck at any point just guides them here to this guide and if you find it helpful then do share it with your geeky programmers’ community and friends.

Though we have tried to cover almost everything as a programmer it’s your responsibility as well to keep looking on to the original documentation of these languages over the internet for better knowledge.

Link: https://developer.mozilla.org/en-US/docs/Web/JavaScript

<h2>What are JavaScript Engines??</h2>
  
Actually, before writing code in JavaScript, you need to know where we are gonna write and run our code and probably, you might be excited about that, so hold on for a moment first let’s move through the software needs first. 

So, for writing the code we will be using VS Code (Visual Studio Code), which is the favorite of most people and gaining a whole lot of popularity. There are a lot of themes and plugins that we can install. Though you can also use codepen.io (Brackets.io – offline version) or sublime for the same purpose no issues.

So, let’s start now:
1.	So, create a folder probably with name ‘Js’ and within it create another folder name ‘hello’, feel free to name it however you like.
2.	Fire up (Open) the VS (Visual Studio) Code.
3.	Drag and drop the ‘hello’ folder over VS Code if you are still following what’s mentioned.
4.	Now the classic way since the ages that have been continuously followed is creating the 2 files namely:
5. 	Within index.html write the following code:

(1) index.html (2) script.js 


```HTML
   <!doctype html>
   <html lang=’en’>
   <head>
	  <meta charset=”UTF-8”>
	  <title>Document</title>
   </head>
   <body>
   Some content is to be added here, wait hold on.
   </body>
   </html>
```
6. It's completely Ok to have the script.js file empty
7. Now add these two lines in betwwen the opening and closing tags of the body.	

```HTML
   <script src = ”script.js”></script>
   <h1> Hello World</h1>
```
8. Go to the file and Open it with Web Browser and you will see Hello World written in big headings over there, but there’s nothing to do with Js as the script.js file is empty.
9. Now right click on the browser screen of page, a drop-down menu select ‘Inspect’/’Inspect element’ and go to console option than.

![Alt](https://github.com/amandewatnitrr/blog/blob/master/_posts/Js_Tutorial_Images/js1.PNG)

10. Now once you are done with this part, go to script.js over VS Code.
11. In the script.js in VS Code write the following line as shown and save it:

```JavaScript
console.log("Hello JavaScript");
```
13. As soon as you save it and reload the page by clicking on the reload button, over the console we see “Hello JavaScript” written over there. This is the proof we can load up our JavaScript in the HTML file.
14. This brings us to a very important question,” Is it the right way to run the JavaScript Code??”

Yeah! It’s fine, all clear 100% there’s no problem with it. But this is not the only way to run the JavaScript and we need to know why this is all happening and how can I run the same code in a bit advanced manner??

![Alt](https://github.com/amandewatnitrr/blog/blob/master/_posts/Js_Tutorial_Images/js2.PNG)

So First of all, we need to understand JavaScript is just like other languages like C++, Java, or Python. It needs a certain thing, tool or set of software so that this JavaScript language can be converted into Machine-Level Language and that’s the most foundation of running the JavaScript and since the very history long we have always seen that the JavaScript comes with a compiler that converts JS code into executable code. Nobody bothers that there’s a compiler running our code. The fact is this engine was already having compilers and people think that they can be run only over browsers. Some of the JavaScript Engines namely are ‘V8’ and ‘Spider Monkey’.

V8 is Google’s Open Source High-Performance JavaScript and WebAssembly engine, written in C++. It is used in Chrome and Node.js among others. It implements ECMAScript and WebAssembly and runs on Windows 7 or later, macOS 10.12+, and Linux system that uses x64, IA-32, ARM, or MIPS processors. V8 can run standalone or can be embedded into any C++ application.

Spider Monkey is Mozilla’s JavaScript engine written in C and C++. It is used in various Mozilla Products, including Firefox, and is available under the MPL2. 

There is no shortage for such JS engines, just like C++ for which we have no. of compilers out there. Things like Node.js are one such implementation that converts your standalone JavaScript code so that we always don’t have to attach our JavaScript to HTML and hit a reload every time. That’s painful that’s why we are not doing it.

<h2>DOM (Document Object Model)</h2>

Now let’s have a bit of knowledge about the DOM Structure of Web Document. JavaScript in addition to getting data from the browser also allows you to manipulate DOM that browsers use to create Web pages.

Every Webpage can be broken down into a mathematical tree structure called the Document Object Model (DOM). Each HTML tag is a node in the tree and these nodes have all types of different attributes such as text, background color, width, etc.

Nodes have properties, methods, and events. Methods here means functions and events refer to various happenings like hover over a link, clicking a button, etc. The Page content of the website is represented by DOM. (Scripting Language) JavaScript uses DOM to interact with the document. Accessing the DOM is done with an API (Application Programming Interface). API is browser-independent.

•	Document - It is the root of the page<br>
•	Element - A node in the tree<br>
•	nodelist - An array or group of elements<br>
•	attribute - A node in DOM though rarely used that way. It provides another way to manipulate or change the document.<br>

Before closing on this topic and moving to the next module let’s talk about Interactivity and how JavaScript does that in our Website. So, HTML5 and CSS3 are not interactive. JavaScript can read and write HTML elements, react/respond to events, validate data, detect visitors, and create cookies.


<h2>ES Version of JavaScript that’s fit</h2>
Like other Languages, JavaScript has a whole of versions of JavaScript, so this question is pretty often okay to arise which one we must use. Some just came into the picture, some offered drastic changes, some offered slight changes, so which one we should be bothered about.

Before moving further let’s have a look at something that almost everyone knows about JavaScript. As mentioned in the previous article, JavaScript has a great power of DOM Manipulation.

So, as you can see here through this diagram it’s clear how 
the web documents are associated with each other.

![Alt](https://github.com/amandewatnitrr/blog/blob/master/_posts/Js_Tutorial_Images/HTML_CSS_JS.PNG)

<h3>ECMAScript</h3>
In the earlier days, there were a lot of scripting languages that were coming up and by scripting languages, we are not referring to bash-trial or Pearl. In this entire scripting world, languages like ActionScript, JavaScript, Jscript, Gscript, and a whole bunch of other languages keep on coming and they were competing with each other. For all the browsers it was getting hard to support all of them, so the European Union (European Computer Manufacturing Association) came into the picture, and then ECMAscript came into the picture. They tried to unify things as one so that things can be done and brought together efficiently, they brought out a set of rules, instructions, and guidelines and this gave rise to ECMAscript. JavaScript is one of the languages which follows the ECMAscript guidelines. The major change came into the picture from ES5 and ES6 onwards. ES6 came into the year 2015 and ES8 in 2018. You might be thinking of working with ES10 or probably even the latest ones. It’s not a great idea to directly jump to ES10 because they are all majorly backward compatible, but the latest browsers supporting there features not possible. So, we will be going through the basic/general version of JavaScript which is even before ES6 and then we will move forward into the features which are available in ES7, ES10.


<h3>Variables and Datatypes in JavaScript</h3>
Let’s just say we want to build an application for your college so for this I would need to reserve some space in the memory. So, let’s say we want to store the roll number of a single student only for now, so I have to allocate some memory for storing the student’s roll number and I will give a unique name to that memory allocated for storing data, this is what we call variable. Variables are named memory allocations used for storing data. A Variable has a memory address and some value associated with it. A variable name can consist of letters, digits, underscores, and ($) sign which is pretty unique in case of JavaScript compared to other languages. Variables cannot start with a digit. JavaScript is a case-sensitive language i.e. ‘roll’ and ‘Roll’ are treated differently. Variable Names should be meaningful.

So, for this purpose we have 3 keywords basically that we will be seeing several times: ‘var’, ’let’, and ‘const’. ‘var’ keyword is used to declare a variable. In JavaScript, we don’t have separate variable type declarations.


Thus, if you are someone who has worked on some other programming language, note for you guys that in Js there is no such difference in technique of variable declaration for decimal, integer, boolean, and string. For most of the cases, we have discussed and pretty much sure you might have understood the concept. So, as in the case, there are many data types in JavaScript and for that, you need to explore the internet knowing about all of them. During the discussion about Variable’s there’s an assignment so if you did it than superb and you might be surprised to see “undefined” rather than getting an error or something like that, it’s like a NULL value telling that till now the memory is allocated to the variable but no value has been assigned to the variable.

![Alt](https://github.com/amandewatnitrr/blog/blob/master/_posts/Js_Tutorial_Images/js4.PNG)
![Alt](https://github.com/amandewatnitrr/blog/blob/master/_posts/Js_Tutorial_Images/js5.PNG)

Code:
```Javascript
var name = "Aman"; //We can store string in here
console.log(name); //Prints the name
var number = 5; //store integer type
var decimal = 5.5;
var bool = true;
console.long(bool);
```

As far we have discussed variable declaration using ‘var’ slowly through implementation we will try to cover up ‘let’ and ‘const’ as well. So, first, let’s discuss ‘const’ keyword. ‘const’ is also used to declare variables but it locks the value in that particular memory address. 

```Javascript
const uid = “abc123”; // Nowhere in this case the value of uid can never be changed even if we desire to do 
```

i.e. it says ok uid is the variable name with some space assigned in memory, you can use it for processing but you can’t change the value in uid.

![Alt](https://github.com/amandewatnitrr/blog/blob/master/_posts/Js_Tutorial_Images/js5.PNG)
